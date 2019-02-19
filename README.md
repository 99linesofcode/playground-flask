# Playground-Flask
This repository contains the boilerplate necessary to setup Flask (a Python Microframework) and interface with NGINX via uWSGI and a TCP/IP socket connection. Though setting up a UNIX socket connection between containers is preferable as it allows for much faster communication, I was unable to get that working at the time of writing this code.

**To be improved**
1. Use the `docker.sock` UNIX socket connection to link multiple containers together and dramatically improve the rate of communication between NGINX and Python containers. 

## Usage
The code in this repository can simply be plugged into [Docker-NGINX-Python-MySQL](https://github.com/99linesofcode/docker-nginx-python-mysql) and served by running one of the make commands that can be found in that repository. Just copy and paste the contents of the `back/` and `front/` directories and you are good to go.

## Contributing
Is there anything that you found to be unclear or would like to see added or rectified? I encourage you to contribute by creating an issue or submitting a pull request. In order to submit a PR, simply:

1. Fork the project
2. Create a new branch with the proposed changes (`git checkout -b <branch name>`)
3. Commit the changes
4. Push the code
5. Create PR for code review

## License
The code in this repository is licensed under the [MIT license](https://opensource.org/licenses/MIT)