# Hands on with Kubernetes Workshop Series - GKE

The following repository will help you create a Kubernetes cluster running on Google Container Engine:

1. Sign up for a Google Cloud account:
    1. FREE TRIAL: $300 of Google Cloud for 12 months https://cloud.google.com/free/
    2. FREE KUBERNETES TIER: up to 5 nodes of Google Container Engine (GKE) are free. Note the underlining Google Compute Engine counts towards the $300 from the FREE TRIAL. 
    3. Keep the Google Cloud console open once you signed up: https://console.cloud.google.com/ 
2. Click link to navigate in the Google Cloud Console to API Manager > Library https://console.cloud.google.com/apis/library. Enable the Compute Engine and Container Engine API: 
![Compute and Container Engine](http://i.imgur.com/obCh0lP.png)
![Enable APIs](http://i.imgur.com/BThkhfK.png)
3. For this workshop we will use the Google Cloud Shell but you might want to consider installing the Google Cloud SDK later (available for Mac, Linux or Windows): https://cloud.google.com/sdk/ for a local command-line client. 

## Create Infrastructure & Provision Cluster

A list of steps to build and provision the Kubernetes cluster can be found [here](docs/3-build-cluster.md)

## Using Kubernetes

The presenter will go through a list of demos during the workshop.

Find the demos [here](docs/demos)


## Destroying Cluster and Load Balancers After Training

Congrats on finishing the hands on introduction to Kubernetes!

To remove the Kubernetes cluster and underlying infrastructure execute the following from the Google Cloud Shell

```
gcloud container clusters delete k8sworkshop --zone=us-east1-c
```

Navigate to the network section in the Google Cloud Portal and delete the load balancers that were created https://console.cloud.google.com/networking/loadbalancing/loadBalancers/ 

You will still have roughly $300 in Google Cloud credits that you can use to play around with Kubernetes some more!



