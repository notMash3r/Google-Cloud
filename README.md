# Google-Cloud

gcloud container clusters create orca-cluster-748 --num-nodes 1 --master-ipv4-cidr=172.16.0.64/28 --network orca-build-vpc --subnetwork orca-build-subnet --enable-master-authorized-networks  --master-authorized-networks 192.168.10.2/32 --enable-ip-alias --enable-private-nodes --enable-private-endpoint --service-account orca-private-cluster-643-sa@qwiklabs-gcp-01-d803bb5018b7.iam.gserviceaccount.com --zone us-east1-b
