# EKS

### EC2에 k8s-mng-server 준비
1. aws cli installation \
  $ sudo apt-get install -y unzip \
  $ curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" \
  $ unzip awscliv2.zip \
  $ sudo ./aws/install \
  $ aws --version

2. eksctl installation
  $ curl --silent --location "https://github.com/weaveworks/eksctl/releases/latest/download/eksctl_$(uname -s)_amd64.tar.gz" | tar xz -C /tmp \
  $ sudo mv /tmp/eksctl /usr/local/bin \
  $ eksctl version
  
3. kubectl installation
  $ curl -o kubectl https://amazon-eks.s3.us-west-2.amazonaws.com/1.19.6/2021-01-05/bin/linux/amd64/kubectl \
  $ chmod +x ./kubectl \
  $ mkdir -p $HOME/bin && cp ./kubectl $HOME/bin/kubectl && export PATH=$PATH:$HOME/bin \
  $ echo 'export PATH=$PATH:$HOME/bin' >> ~/.bashrc \
  $ kubectl version --short --client  

4. 
