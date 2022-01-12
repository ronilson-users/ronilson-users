cd ~/.ssh
ls -la ~/.ssh/id_rsa*
cp ~/.ssh/id_rsa ~/.ssh/id_rsa.old

$ mkdir key_backup
# Makes a subdirectory called "key_backup" in the current directory

$ cp id_rsa* key_backup
# Copies the id_rsa keypair into key_backup

$ rm id_rsa*
# Deletes the id_rsa keypair

ssh-keygen -t rsa -b 4096 -C "ronilson.stos@gmail.com"
ssh-keygen -t rsa -C "your_email@youremail.com"
ssh -T git@github.com

