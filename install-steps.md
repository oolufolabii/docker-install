# Install packages
$ sudo apt-get install apt-transport-https ca-certificates curl software-properties-common
# Add Docker’s official GPG key:
$ wget https://download.docker.com/linux/ubuntu/gpg
$ sudo apt-key add gpg
# Verify that you now have the key with the fingerprint
$ sudo apt-key fingerprint 0EBFCD88
 '''   pub   rsa4096 2017-02-22 [SCEA]
          9DC8 5822 9FC7 DD38 854A  E2D8 8D81 803C 0EBF CD88
    uid           [ unknown] Docker Release (CE deb) <docker@docker.com>
    sub   rsa4096 2017-02-22 [S]
 '''
# Set up the stable repository
$ sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
# Update the apt package index
$ sudo apt-get update
# Install the latest version of Docker CE
$ sudo apt-get install docker-ce
$ sudo apt-get install docker-ce docker-ce-cli containerd.io
# confirm version
$ sudo docker version
