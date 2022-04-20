# Here is how we can copy ssh id using pem

```
cat ~/.ssh/id_rsa.pub | ssh -i /mnt/f/ssh_keys/descpro-azure_key.pem  ubuntu@<ip> "cat - >> ~/.ssh/authorized_keys"
```

# how to run script on the remote machine using ssh 
https://stackoverflow.com/questions/305035/how-to-use-ssh-to-run-a-local-shell-script-on-a-remote-machine

```
ssh root@MachineB 'bash -s' < local_script.sh
```
For a script that requires sudo, run ```ssh root@MachineB 'echo "rootpass" | sudo -Sv && bash -s' < local_script.sh.``` 
