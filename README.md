# Simplerisk
# scripted Install 

Option 1: SimpleRisk Scripted Installation

Run this command as "root" on a newly provisioned system to perform a scripted SimpleRisk installation:
curl -sL https://raw.githubusercontent.com/simplerisk/setup-scripts/master/simplerisk-setup.sh | bash -

Currently supported Operating Systems include:
Ubuntu 22.04
Ubuntu 20.04
CentOS 8
CentOS 7
SLES 15
RHEL 9
RHEL 8
Debian 11


Option 2: SimpleRisk Virtual Machine Installation

VMWare Virtual Machine
1) Download the Virtual Machine Image:
SIMPLERISK 20250411-001 VIRTUAL MACHINE (VMWare)
2) Validate the Checksum:
MD5 Checksum = 96eb00b874bc77ff5fc95752398edfcb
3) Install the Virtual Machine:
INSTALL SIMPLERISK AS A VMWARE APPLIANCE
4) Secure the Virtual Machine:
SECURE YOUR SIMPLERISK VIRTUAL MACHINE
VirtualBox Virtual Machine
1) Download the Virtual Machine Image:
SIMPLERISK 20250411-001 VIRTUAL MACHINE (Virtualbox)
2) Validate the Checksum:
MD5 Checksum = f4b358cfaadaba57f0e280d4eb13a961
3) Install the Virtual Machine:
INSTALL SIMPLERISK AS A VIRTUALBOX APPLIANCE
4) Secure the Virtual Machine:
SECURE YOUR SIMPLERISK VIRTUAL MACHINE

Option 3: SimpleRisk Docker Installation

DockerHub Image
1) Download the SimpleRisk image from DockerHub:
docker pull simplerisk/simplerisk
2) Start the Docker Container:
docker run --name simplerisk -d -p 80:80 -p 443:443 simplerisk/simplerisk
3) Test Your SimpleRisk Instance:
https://localhost/
Compiled Docker Image
1) Clone the SimpleRisk Docker Repository:
git clone https://github.com/simplerisk/docker.git simplerisk-docker
2) Change to the Docker directory:
cd simplerisk-docker/simplerisk
3) Build the SimpleRisk Docker Image:
docker build -t simplerisk/simplerisk -f noble/Dockerfile .
4) Start the Docker Container:
docker run --name simplerisk -d -p 80:80 -p 443:443 simplerisk/simplerisk
5) Test Your SimpleRisk Instance:
https://localhost/

Option 4: SimpleRisk Manual Installation

WARNING: A SimpleRisk Manual Installation requires following a precise set of instructions which are conveniently performed for you with our other installation methods. Operating systems updates are frequent and these instructions can only serve as guidance for the point in time when they were written. You may need to make modifications for SimpleRisk to work in your environment. As such, this installation method should only be used in situations where running Ubuntu is not an option or the environment necessitates a non-standard configuration.


1) Download the Web Bundle:
SIMPLERISK 20250411-001 WEB BUNDLE
2) Validate the Checksum:
MD5 Checksum = 2ce0cee46afeef101d2c3fbd2130c977
3) Follow the Instructions:
INSTALL SIMPLERISK ON UBUNTU 22.04 (APACHE/MYSQL/PHP)
INSTALL SIMPLERISK ON UBUNTU 20.04 (APACHE/MYSQL/PHP)
INSTALL SIMPLERISK ON CENTOS 8 (APACHE/MYSQL/PHP)
INSTALL SIMPLERISK ON REDHAT ENTERPRISE LINUX 8 (APACHE/MYSQL/PHP)
INSTALL SIMPLERISK ON WINDOWS 8/10 USING WAMP SERVER
