## Step 1 — Create Resource Group

Created a new resource group:

vm-web-01_group


## Step 2 — Deploy Ubuntu VM

Configuration:

Region: West Europe
Size: Standard D2s v3
Image: Ubuntu 24.04 LTS
Authentication: SSH key


## Step 3 — Connect to VM

ssh -i ~/.ssh/id_ed25519 azureuser@PUBLIC_IP


## Step 4 — Install Nginx

sudo apt update
sudo apt install nginx -y


## Step 5 — Start Nginx

sudo systemctl start nginx
sudo systemctl enable nginx
