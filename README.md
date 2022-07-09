# ft_server
[![tclement's 42 ft_server Score](https://badge42.vercel.app/api/v2/cl59lbrtc003009jqom2qgm4z/project/2004454)](https://github.com/JaeSeoKim/badge42)<br>

# ft_server
***This is a System Administration project. This project uses Docker technology to set up a web server, which will run multiple services (```Wordpress```, ```PhpMyAdmin```, ```MySQL```).***

The project also demonstrates the importance of using scripts to automate tasks. 

## Technical considerations

- ```Docker-compose``` is not allowed
- Container OS must be ```debian buster```
- The server needs to use the ```SSL``` protocol
- The server ```redirects``` to the correct website based on the url

## How to test
> Run the following commands while running Docker

```shell
$ git clone https://github.com/DelicaTessa/42-ft_server
$ cd 42-ft_server
$ docker build -t ft_server .
$ docker run -it -p 80:80 -p 443:443 ft_server
