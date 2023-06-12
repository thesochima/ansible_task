# ansible_task
From the aws console i was able to navigate to the 'ec2 dashboard' and i  clicked on 'launch instance' 
and during the process of creating the instance i selected  the t2 micro free tier instance
the ubuntu 20.04 AMI "amazon/ubuntu/images/hvm-ssd/ubuntu-focal-20.04-amd64-server-20230517" was selected to prioritize stability.
I created a key pair to securely connect to the instance.
A security group was created to allow ssh traffic and https traffic to the instance.
I configured a 8GB gp2 EBS for the instance and launched the instance.

Another ec2 instance with the same configurations was created named "ansible_server" with the inventry file in the home directory
The playbook script is in the test.yaml file also in the home directory   
The required nice-script.sh is also in the home directory.
to run the ansible playbook as seen in the git repository, run the "ansible-playbook -i inventory test.yaml"

