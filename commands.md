# Commands Used

This file contains the main commands used to deploy and configure an Nginx web server on an Azure Linux virtual machine.

---

## 1. Generate SSH Key

Generate a new SSH key pair for secure authentication.

```bash
ssh-keygen -t ed25519
```

---

## 2. Connect to the Azure Virtual Machine

Use the generated SSH key to connect to the VM.

```bash
ssh -i ~/.ssh/id_ed25519 azureuser@<public-ip-address>
```

---

## 3. Update Package Repository

Update the system package index before installing new software.

```bash
sudo apt update
```

---

## 4. Install Nginx

Install the Nginx web server.

```bash
sudo apt install nginx -y
```

---

## 5. Start and Enable Nginx

Start the Nginx service and configure it to start automatically on boot.

```bash
sudo systemctl start nginx
sudo systemctl enable nginx
```

---

## 6. Verify Nginx Status

Check the status of the Nginx service to ensure it is running.

```bash
sudo systemctl status nginx
```
