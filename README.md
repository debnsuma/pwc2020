# pwc2020

git clone https://github.com/debnsuma/pwc2020.git

Demo App 
--------

# Set up a Python virtual environment with flask

- mkdir demo
- cd demo
- virtualenv virt
- source virt/bin/activate
- pip install flask==1.0.2
- pip freeze > requirements.txt

# Create a flask application

- vim application.py   # call the object as app for python3.7
- python application.py  
- Open http://127.0.0.1:5000/ in your web browser

# Deploy your site with the EB CLI

- vim .ebignore 
- eb init -p python-3.7 demo --region us-east-1
------------------------------
Check in UI > EB > Application 
------------------------------

- eb create flask-env
- eb open 

Wine Quality Predector
----------------------

- cd eb-flask
- pip install -r requirements.txt
- python application.py 
- Open http://127.0.0.1:5000/ in your web browser

# Deploy your site with the EB CLI
- eb init -p python-3.7 winedemo --region us-east-1
- eb create flask-env-winedemo
- eb open 