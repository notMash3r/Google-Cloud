# Google-Cloud

<br/><br/>
---Creating a Security Custom Role---
<br/>
nano role-definition.yaml

Edit this into YAML file: <br/>

title: "Enter Your_Service_Account"   <br/>
description: "Permissions"<br/>
stage: "ALPHA"<br/>
includedPermissions: <br/>
&ndash; storage.buckets.get<br/>
&ndash; storage.objects.get<br/>
&ndash; storage.objects.list<br/>
&ndash; storage.objects.update<br/>
&ndash; storage.objects.create<br/>



---Creating a Private Cluster--- <br/><br/>
gcloud container clusters create <Your Cluster_Name> --num-nodes 1 --master-ipv4-cidr=172.16.0.64/28 --network orca-build-vpc --subnetwork orca-build-subnet --enable-master-authorized-networks  --master-authorized-networks 192.168.10.2/32 --enable-ip-alias --enable-private-nodes --enable-private-endpoint --service-account <Your Service Account Name>@<Your Qwiklabs PROJECT ID>.iam.gserviceaccount.com --zone us-east1-b
  
<br/><br/>
---Deploy an Application to Kubernetes Engine Cluster---
gcloud container clusters get-credentials orca-cluster-748 --internal-ip --zone us-east1-b --project qwiklabs-gcp-01-d803bb5018b7
           
