---------------------- K8S --------------------------
kubectl run nginx --image nginx (will create a pod with nginx running on it)

kubectl get pods (Will list all pods in default namespace)



---------- K8S yaml file-------------------
- Muat have parameter in K8S manifestfile

apiVersion: (This state the version of k8s api we want to use for this manifest file or definition files)

EG:
- KIND                          apiVersion
	- Pod                         v1
	- Service                     v1
	- ReplicaSet                  app/v1       
	- Deployment                  app/v1 
kind:
metadata: (this section refers to all information about the file
	EG:
		name: yourappname
		labels: (can add whatever key value paire you want)
			app: yourappname
			type: front-end
spec:
	containers: (is a list or dictionary, which can contain mant contaners)
		- name: nginx-server
		  image: nginx

======= assume our manifest file name is 'pod-deploy.yml, to run the pod,use ========

	kubectl create -f pod-deploy.yml OR 	kubectl apply -f pod-deploy.yml (can be use to update data on running pods 'apply'
	kubectl get pods (to check the creation of the pods) OR -o wide
	kubectl describe pod yourappname (provides detailed information about the pod)




====== demo (app.yml) ====

apiVersion: v1
kind: Pod
metadate:
  name: nginx
  labels:
    app: nginx
    tier: fronend
spec:
  containers
  - name: nginx
    image: nginx
  - name:anotherPod
    image: busybox 


======== auto generate definition file ============
kubectl run httpd --image=httpd --dry-run=client -o yaml > httpd.yaml



============ ReplicaSets (Replication Controller) =================
Help to bring up a new pods when ever the existing pod fails

Its also help to auto-scale our pods to meet user demands.


===== replicationcontroller-definition.yml ==================

apiVersion: apps/v1
kind: ReplicaSet
metadate:
  name: myapp-replicaset
  labels:
    app: myapp
    tier: frontend
spec:
  template:
    metadate:
       name: nginx
       labels:
         app: nginx
         type: fronend
    spec:
     containers
     - name: nginx
       image: nginx

  replicas: 4
  selector:                    (selects and manages all lable specified here)
    matchLabels:
       type: frontend


==run 'kubectl create -f replicaset-definition.yml' to create the replica set

to get the pods in the replica set
	run 'kubectl get replicationController



===== replicaset-definition.yml ==================

apiVersion: v1
kind: ReplicationController
metadate:
  name: myapp-replicaset
  labels:
    app: myapp
    tier: fronen
spec:
  template:
    metadate:
       name: nginx
       labels:
         app: nginx
         type: fronend
    spec:
     containers
     - name: nginx
     image: nginx

  replicas: 4
   selector:
    matchlable:
       type: frontend



=== Commands ===
kubectl get replicaset

kubectl replace -f filename.yml (when you have change the replicaset number in the definition file.)

  OR

kubectl scale --replicas=10 -f filename.yml

kubectl get replicaset (or 'rs' = replicaset)

kubectl explain replicaset (will provide not on how to write a definition file for a replicaset

kubectl delete replicaset app-name


NOTE:
	when ever you edit and update a definition file or runing pods, all you need to do is to delete all the older pods and the relicaset will automatically create new relicasets with the new update.
