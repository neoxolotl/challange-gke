README
======
./start                                                                 User Commands                                                                 start
       ./start - Install Terraform and modules for Google Provider and deploy Cluster.

SYNOPSIS
       ./start [OPTION]... [COMMANDS]...
       ./start [OPTION] []...

OPTIONS
       Install Terraform and modules for Google Provider and deploy Cluster 
       Mandatory arguments to long options are mandatory for short options too.

       -p, --provision

       -tf, --Terraform choice install 

        	L, --Linux - Install and Initialize Terraform on Linux
        	M, --MacOs - Install and Initialize Terraform on MacOS - beta
		  
COMMANDS
	CREATE, --Create Install Terraform + Google Modules. 
	
	DESTROY, --Destroy from Terraform Cluster. 

	OUTPUT, --Output

	--help, --Help you 
		
Example
=======	
	./start -p CREATE -tf L	
				(Install Terraform on Linux and deploy Cluster)
					
	./start -p CREATE -tf M
				(Install Terraform on MacOs and deploy Cluster) 









Requeriments
==============

Unzip 

apt install unzip 


cd terraform

Init modules 

terraform init 





This documentations 

1.- Install Terraform
=========================


Linux
======

wget https://releases.hashicorp.com/terraform/0.12.6/terraform_0.12.6_linux_amd64.zip
unzip terraform_0.12.6_linux_amd64.zip
sudo mv terraform /opt/terraform
sudo ln -s /opt/terraform /usr/local/bin/terraform

	Initialize
	----------

echo "deb https://packages.cloud.google.com/apt cloud-sdk main" | sudo tee -a /etc/apt/sources.list.d/google-cloud-sdk.list
curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
sudo apt-get update && sudo apt-get install google-cloud-sdk kubectl
gcloud init 




MacOS
==========

brew install terraform

	Initialize
	----------

curl https://sdk.cloud.google.com | bash
exec -l $SHELL
curl -LO https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/darwin/amd64/kubectl
chmod +x ./kubectl && sudo mv ./kubectl /usr/local/bin/kubectl
gcloud init












API-KEY 
========

AIzaSyDFLr3jI-KJfoIw8-_ZDEuJEut-8Ug-Edc


Para usar esta clave en tu aplicación, debes transferirla con el parámetro key=API_KEY.




Clave de API Undefined parameter - RECUENTO



Api-key 

AIzaSyDFLr3jI-KJfoIw8-_ZDEuJEut-8Ug-Edc





Links: 

