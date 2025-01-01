/// Google cloud commands ///

* Set region: 
  - gcloud config set compute/region REGION 

  > Ej.: gcloud config set compute/region us-central1
____________________________________________________________________________

* View the project region setting:
  - gcloud config get-value compute/region
____________________________________________________________________________

* Set zone: 
  - gcloud config set compute/zone ZONE 

  > Ej.: gcloud config set compute/zone us-central1-c
____________________________________________________________________________

* View the project region setting:
  - gcloud config get-value compute/zone
____________________________________________________________________________

* View project ID:
  - gcloud config get-value project
____________________________________________________________________________
* View details about the project:
  - gcgcloud compute project-info describe --project $(gcloud config get-value project)
____________________________________________________________________________