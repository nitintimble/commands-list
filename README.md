# commands-list
miscellaneous commands

## chmod 400 alternative for windows


open powershell from folder where key is present

icacls.exe .\timble_human_dev_key.pem /reset

icacls.exe .\timble_human_dev_key.pem /grant:r "$($env:USERNAME):(r)"

icacls.exe .\timble_human_dev_key.pem /inheritance:r

## VS Code: NoPermissions (FileSystemError): Error: EACCES: permission denied

sudo chown -R emanuel /home/emanuel/test/

SSH windows to Ec2
ssh -i "D:\aws-key\dev_key.pem" ubuntu@ec2-3-111-193-227.ap-south-1.compute.amazonaws.com
