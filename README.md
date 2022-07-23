# CI/CD-poc
CI/CD proof of concept

- set var for your service account 
 	`export SERVICEACCOUNT=""`
- Command for Jenkins principal node cration - Centos 7
	`gcloud compute instances create jenkins-nodo-principal --project=$GOOGLE_CLOUD_PROJECT --zone=us-central1-f --machine-type=e2-micro --network-interface=network-tier=STANDARD,subnet=default --service-account=$SERVICEACCOUNT --scopes=https://www.googleapis.com/auth/cloud-platform --create-disk=auto-delete=yes,boot=yes,device-name=jenkins-nodo-principal,image=projects/centos-cloud/global/images/centos-7-v20220621,mode=rw,size=20,type=projects/$GOOGLE_CLOUD_PROJECT/zones/us-central1-f/diskTypes/pd-standard --preemptible`

- Install Jenkins: https://www.jenkins.io/doc/book/installing/linux/#red-hat-centos
