# commands-list
miscellaneous commands

## ERROR: Could not install packages due to an OSError: [Errno 28] No space left on device

pip cache purge

## Environment - v s code - bitbadh - windows

python -m venv venv

source venev/scripts/activate

## chmod 400 alternative for windows


open powershell from folder where key is present

icacls.exe .\timble_human_dev_key.pem /reset

icacls.exe .\timble_human_dev_key.pem /grant:r "$($env:USERNAME):(r)"

icacls.exe .\timble_human_dev_key.pem /inheritance:r

## VS Code: NoPermissions (FileSystemError): Error: EACCES: permission denied

sudo chown -R ubuntu usr/local/code/

sudo chown -R user folder-path


## SSH windows to Ec2
ssh -i "C:\Users\nitin\.ssh\dev_key.pem" ubuntu@ec2-3-111-193-227.ap-south-1.compute.amazonaws.com

## Terminate the Existing Process (Error: listen EADDRINUSE: address already in use :::3000)
sudo lsof -i :3000


sudo kill -9 < PID >

## vd code ssh connect ec2

icacls C:\Users\nitin\.ssh\dev_key.pem /inheritance:r


icacls C:\Users\nitin\.ssh\dev_key.pem /remove:g "NITINM-LTP\Admin account"


icacls C:\Users\nitin\.ssh\dev_key.pem /grant:r "NITINM-LTP\nitin:(R)"


## check ram available on ec2

free -h

## create swap ec2

### Create swap file:
sudo fallocate -l 4G /swapfile

### Set permissions:
sudo chmod 600 /swapfile

### Set up swap space:
sudo mkswap /swapfile

### Enable swap:
sudo swapon /swapfile

### Make swap file permanent:
sudo echo '/swapfile none swap sw 0 0' | sudo tee -a /etc/fstab



