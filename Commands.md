AWS VOLUME EXTRA MOUNT 

lsblk

sudo df -h

sudo mkfs -t xfs /dev/xvdb

sudo mkdir /additional

sudo mount /dev/xvdb /additional/

lsblk

sudo df -h

sudo blkid

sudo lsblk

IN LOCATION vi /etc/ftstab

UUID=b059909f-ab05-4a3c-a142-018ca902359d /additional   xfs   defaults,nofail   1   2


### DOCKER COMMANDS

docker image build -f myimageinstuctions .

docker image build -f myimageinstuctions ~/nn

curl -fsSL https://get.docker.com -o get-docker.sh

sh get-docker.sh


docker image build -t spc_two:1.0 .

docker container run --name processtwo -d -P spc_two:1.0

docker container rm -f $(docker container ls -a -q)

docker image rm -f $(docker image ls -q)



aws ec2 run-instances \
    --image-id ami-03b755af568109dc3 \
    --instance-type t2.micro \
    --key-name mine
	
create-security-group
--description hello
--group-name hi

aws ec2 authorize-security-group-ingress --group-id sg-026c86352cc7d8221 --protocol tcp --port "-65535" --cidr 0.0.0.0/0


grep "2015-12-19.*.install " /var/log/dpkg.log | awk '{ print $4 }' | cut -d: -f1 | xargs sudo apt-get --yes purge


export PATH="/usr/lib/jvm/java-1.8.0-openjdk-amd64/bin:$PATH"

export PATH="/opt/apache-maven-3.6.3/bin:$PATH"

find ~/ -name \*.jar



%USERPROFILE%\AppData\Local\Packages\Microsoft.Windows.ContentDeliveryManager_cw5n1h2txyewy\LocalState\Assets : Location of the spotlight wallpapers.

