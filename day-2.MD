# Server Basics & EC2 Setup Guide

---

## Server:
windows Vs Linux -> linux has more speed than windows  
- windows is graphics based  
- linux is command based and everything is text  
- less power  
- less bandwidth  
- less memory  
- 100% free  
- fast  

---

### Example: https://facebook.com
- Protocol: https  
- Port: 443  
- IP: DNS IP  
- Then we enter Username and password --> Authentication  

If a person connects to server needs to connect: 12qe  
SSH -> secure shell -> Linux Authentication mechanism  
port no is 22  

---

## Authentication Mechanism:
1. what you know  
2. what you have  
3. what you are  

**1. what you know**  
- username & password  

**2. what you have**  
- keys or tokens (RSA physical tokens)  

**3. what you are**  
finger frint, retina, palm -> As of now we don't have this technology   
to access remote servers, hope for best in future  

As of now we are following   
- user name & password  
- user name & private key  

---

## what are keys??
- public key Vs private key  
- public key and private key is more secure than username & password  

---

## Linux server launch:
Linux -> introduced by linux torvalds and also Git  
Before linux we have unix  

linux torvalds was worked in Unix team  
he noticed that unix strictly coupled with hardware  

is that possible to run MAC OS in Lenevo laptop?  
MAC laptop has software + hardware --> we don't have freedom to choose OS  
If you take any laptop except MAC it's our wish like we can run linux, windows and ubuntu etc..,  
but Unix is not free and high cost  

and windows also we have disadvantages:  
- not open source  
- costly  
- not secure must install anti virus  
- slow  
- too many graphics  
- frequent restarts  
- tough to upgrade/update  

because of this disadvantages he started writing OS from the scratch using C laguage  
- no strict couple with hardware  
- it is free and opensource  

**advantages are:**  
- secure  
- high speed  
- no need of restarts  
- install or update packages is easy  
- free, community support is there  
- low resources  

---

### Linux is OS or Kernel??
Actually it is a kernal, it is a software component that can interact with hardware  
Kernal is the heart of OS  

if we see architecture of linux operating system:  
- first we have hardware (cpu, ram, storage, processor etc..)  
- kernal is interacting with hardware  
- shell is interacting with kernal  
- application & utilities is interacting with shell  

then few companies developed shell to interact with kernal and few utilities  
i.e **kernal + shell + utilities == OS**  

basically linux is a kernal, on this linux kernal so many OS developed.  
we can call it as linux flavours or distributions.  

---

### Flavours / Distributions (OS):
OS is used to interact with hardware.  

- Ubuntu  
- RHEL  
- CentOS  
- Fedora  
- IBM  
- Suse  
- Android  

**In this linux we have two types:**  
1. desktop version, in this we have graphics  
2. server version, in this no graphics only terminal or shell  

---

## EC2 server/box/node launch:
before going to launch EC2 server you should have public key and private key  

first we have to open git bash terminal  
once you opened follow below steps to create public key and private key  

```bash
ssh-keygen -t rsa -b 4096 -f <file-name>
# or
ssh-keygen -f <file-name>

it will generate public key and private key

Create EC2:

EC2 dashboard -> click on lauch instance

Name

select AMI

Instance type

create/import key in AWS account

Firewall/security group creation

launch instance

create/import key in AWS account:

Login to AWS account console
EC2 dashboard -> network security -> key pair
click on actions
import public key pair

Firewall/security group creation:

Login to AWS account console
EC2 dashboard -> network security -> security groups
create security group -> Basic details -> Security group name -> Description

Select Inbound rule : click on add rule

Type

Protocol

Port range

Source

Destination

where you select anywhere ipv4 i.e., 0.0.0.0/0 which means internet, open for everyone
or
my ip i.e., <ip-address>, it will open for your home only

Select Outbound rule : click on add rule

Type

Protocol

Port range

Source

Destination

where you select anywhere ipv4 i.e., 0.0.0.0/0 which means internet, open for everyone
or
my ip i.e., <ip-address>, it will open for your home only

Total Ports

Total we have 65,536 ports available in system i.e., 0-65,535

Lets take real time example:

i am sending a post from bangalore to Hyderabad

in adress we have flat no, apartment name, street, city, pincode

if i give only pincode it will reach to that city it will struck there

if i give street name it will reach to that street it will struck there

if i give apartment name it will reach to that apartment it will struck there

if i didn't mention flat no or owner name it will struck in apartment only

same way in system so many process are running, every process will open one port number..

for example if i give

https://facebook.com:443


which means there is a https process running inside facebook server on port number 443

a random port will be opened for this chrome tab, i want facebook.com on 443, i opened
a random port something like 44565, thats why port number is important

we use firewalls to open and block

do we have access for SSH port number 22? → No, only facebook admin staff will have this access

do we have access for https access? → Yes, public will have this access

what facebook will do you know

they open 443 port for public

they open 22 port for admin staff

Connect to EC2

once you launch the instance open the gitbash terminal

ssh -i <private-key> <user-name>@IP


-> you can able to login into server

and also you can use putty, super putty, mobaxtream software to launch the servers