# ubuntu-psycopg2-setup

Instructions to install psycopg2 in Python 3 virtual environment on Ubuntu 18.04 on AWS.

AMI: Ubuntu Server 18.04 LTS (HVM), SSD Volume Type

## Update OS and install some libraries

sudo apt-get update

sudo apt-get install libpq-dev gcc

## Upgrade to Python 3.7

python3 -V

sudo apt install python3.7

sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.7 1

sudo rm /usr/bin/python3

sudo ln -s python3.7 /usr/bin/python3

python3 -V

## Install some packages for Python3

sudo apt install python3.7-dev

sudo apt install python3-pip

sudo apt install -y python3.7-venv


## Create the virtual environment

python3 -m venv [folder]/venv  -- installs virtual directory "venv" in folder

cd [folder]

source venv/bin/activate

## Install psycopg2

pip3 install psycopg2

