# Google-Cloud

---Creating a Private Cluster--- <br/><br/>
gcloud container clusters create <Your Cluster_Name> --num-nodes 1 --master-ipv4-cidr=172.16.0.64/28 --network orca-build-vpc --subnetwork orca-build-subnet --enable-master-authorized-networks  --master-authorized-networks 192.168.10.2/32 --enable-ip-alias --enable-private-nodes --enable-private-endpoint --service-account <Your Service Account Name>@<Your Qwiklabs PROJECT ID>.iam.gserviceaccount.com --zone us-east1-b
