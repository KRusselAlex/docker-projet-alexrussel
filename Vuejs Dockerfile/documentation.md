To use this dockerfile

## create a vue js app 

```sh
npm create vue@latest

```
#### follow all the step to install what you need to start your vue js app

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
docker run --name "name of your container" -d -p "the port you want to run vue js":80 "name of your image"

```

### finaly run localhost the port you are using 
