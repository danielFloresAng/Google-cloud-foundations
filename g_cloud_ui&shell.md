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

* List the active account name:
  - gcloud auth list
____________________________________________________________________________

* List the project ID:
  - gcloud config list project
____________________________________________________________________________

* Create an environment variable:
 - export VARIABLE_NAME=VALUE

* Create an environment variable to store your Project ID:
  - export VARIABLE_NAME=$(gcloud config get-value project)
  > Ej.: export PROJECT_ID=$(gcloud config get-value project)

* Create an environment variable to store your Zone:
  - export VARIABLE_NAME=$(gcloud config get-value compute/zone)
  > export ZONE=$(gcloud config get-value compute/zone)
____________________________________________________________________________

* se the enviroments variable's value:
  - echo -e $VARIABLE_NAME

> EJ.:
* Verify that your variables were set properly, run the following commands:
  - echo -e "PROJECT ID: $PROJECT_ID\nZONE: $ZONE"
____________________________________________________________________________

* Create a virtual machine:
  - gcloud compute instances create VM_NAME
  > Ej.: gcloud compute instances create gcelab2 --machine-type e2-medium --zone $ZONE
____________________________________________________________________________

* View the list of configurations in your environment:
  - gcloud config list
____________________________________________________________________________

* See all properties and their settings:
  - gcloud config list --all
____________________________________________________________________________

* List your components:
  - gcloud components list
____________________________________________________________________________

* List the compute instance available in the project:
  - gcloud compute instances list
____________________________________________________________________________

* LisList the firewall rules in the project:
  - gcloud compute firewall-rules list
____________________________________________________________________________

* Connect to your VM with SSH:
  - gcloud compute ssh gcelab2 --zone $ZONE
____________________________________________________________________________

* Install nginx web server on to virtual machine:
  - sudo apt install -y nginx
____________________________________________________________________________

* List the firewall rules for the project:
  - gcloud compute firewall-rules list
____________________________________________________________________________


