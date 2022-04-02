# Here is how we can copy ssh id using pem

```
cat ~/.ssh/id_rsa.pub | ssh -i /mnt/f/ssh_keys/descpro-azure_key.pem  ubuntu@<ip> "cat - >> ~/.ssh/authorized_keys"
```
