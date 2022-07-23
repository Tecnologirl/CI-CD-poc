# CI/CD-poc
CI/CD proof of concept

- Centos 7 VM for Jenkins

	`gcloud compute instances create jenkins-nodo-principal --project=technologirl --zone=us-central1-f --machine-type=e2-micro --network-interface=network-tier=PREMIUM,subnet=default --maintenance-policy=MIGRATE --provisioning-model=STANDARD --service-account=jenkins@technologirl.iam.gserviceaccount.com --scopes=https://www.googleapis.com/auth/cloud-platform --create-disk=auto-delete=yes,boot=yes,device-name=jenkins-nodo-principal,image=projects/centos-cloud/global/images/centos-7-v20220621,mode=rw,size=20,type=projects/technologirl/zones/us-central1-f/diskTypes/pd-standard --no-shielded-secure-boot --shielded-vtpm --shielded-integrity-monitoring --reservation-affinity=any	--preemptible`
