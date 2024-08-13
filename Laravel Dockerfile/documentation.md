To use this dockerfile

## create a laravel app 

```sh
composer create-project laravel/laravel "name of app" 

```
#### Follow all the step to install what you need to start your laravel app

#### Copy this dockerfile in the root of the directory

#### on the terminal runthe following command to create the image 

```sh
docker build -t "name of your image" .

```

#### if you have a message like permision denied start your command with sudo and put your password

#### if you want to see the image created type

```sh
docker images

```
## creat a container 

```sh
docker run --name "name of your container" -d -p "the port you want to run vue js":8181 "name of your image"

```

## example 

```sh

 docker build -t laravel-app .
 docker images
 docker run --name laravel-app-container -d -p 8181:8181 laravel-app
 docker ps

 ```



### finaly run localhpst the port you are using 
