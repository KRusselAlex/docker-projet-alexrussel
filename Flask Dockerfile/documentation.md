To use this dockerfile

## create a flask app 

```sh

mkdir myproject
cd myproject
python3 -m venv .venv
. .venv/bin/activate
pip install Flask

```
#### follow all the step to install what you need to start your flask app

### create a requirement to store all dependencies with

```sh

pip freeze > requirement.txt

```

#### Copy this dockerfile in the root of the directory

#### on the terminal runthe following command to create the image 

```sh

docker build -t "name of your image" .

```

#### if you have a message like permision denied start your command with sudo and put your password

#### if you want to see the image created 

```sh
docker images

```
## creat a container 

```sh
docker run --name "name of your container" -d -p "the port you want to run vue js":8000 "name of your image"

```


## example take a docker image called flask-app, you have permission problems use sudo

```sh

 docker build -t flask-app .
 docker images
 docker run --name flask-app-container -d -p 8000:8000 flask-app
 docker ps

 ```


### finaly run localhpst the port you are using 
