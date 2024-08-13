To use this dockerfile

## create a express js app 

```sh
nprm install express

```

### add this in package.json to be able to use ES6

```sh

"type": "module",
```

#### create a file copy ths dockerfile in the root of the directory

#### on the terminal runthe following command to create the image 

```sh
docker build -t "name of your image" .

```
#### NB: dont worry if you see warnings this only means that there are command in dockerfile which are not in capital letter like as you can change to AS

#### if you have a message like permision denied start your command with sudo and put your password

#### if you want to see the image created type

```sh
docker images

```
## creat a container 

```sh
docker run --name "name of your container" -d -p "the port you want to run vue js":3000 "name of your image"

```

## example 

```sh

 docker build -t node-app .
 docker images
 docker run --name node-app-container -d -p 3000:3000 node-app
 docker ps

 ```

### finaly run localhpst the port you are using 
