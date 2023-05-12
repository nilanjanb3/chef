knife ssl fetch

knife ssl check

sudo scp -i vm1key.pem  chef-starter.zip ubuntu@44.192.42.242:/home/ubuntu/temp

knife cookbook upload starter

sudo knife bootstrap 192.168.110.8 --ssh-user root --ssh-password vagrant  -N client.chef.com --sudo

chef-client --version


sudo chef-client