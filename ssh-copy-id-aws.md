# Here is how we can copy ssh id using pem

`
cat ~/.ssh/id_rsa.pub | ssh -i /mnt/f/ssh_keys/descpro-azure_key.pem  ubuntu@20.232.44.27 "cat - >> ~/.ssh/authorized_keys"
`
