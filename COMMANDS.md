knife ssl fetch

knife ssl check

sudo scp -i vm1key.pem  chef-starter.zip ubuntu@44.192.42.242:/home/ubuntu/temp

knife cookbook upload starter

sudo knife bootstrap 172.31.14.147 --ssh-user ubuntu --ssh-identity-file /home/ubuntu/temp/vm1key.pem -N client.example.com --sudo

chef-client --version


sudo chef-client