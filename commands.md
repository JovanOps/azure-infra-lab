ssh-keygen -t ed25519

ssh -i ~/.ssh/id_ed25519 azureuser@PUBLIC_IP

sudo apt update
sudo apt install nginx -y

sudo systemctl start nginx
sudo systemctl enable nginx
sudo systemctl status nginx
