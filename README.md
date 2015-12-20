# torc

[![Build Status](https://travis-ci.org/rascal999/torc.svg)](https://travis-ci.org/rascal999/torc)

Specify targets and run sets of tools against them

torc is designed to make a pentester's life easier and more consistent
by allowing them to specify tools they would like to run against targets,
without having to type them in a shell or write a script. This tool will
probably be useful during certain exams as well..

## Installation

torc is contained in the
[rascal999/torc](https://hub.docker.com/r/rascal999/torc/)
docker image which means all you have to do is download the docker image
and get it running. torc-web (a torc client) is already installed as part
of the docker image, as well as many of the tool dependencies torc has.

This repository is really only useful to you if you want to develop torc.
If you just want to use torc, please see the
[rascal999/torc](https://hub.docker.com/r/rascal999/torc/)
docker image.

Only allow this package to listen on a loopback IP address. If you have
this package listen on a public IP, you're allowing arbitrary users to
execute commands as root on your server. Eventually, HTTPS and credentials
will be required, but for now, don't be a moron.

#### From Docker

1. Execute ``docker pull rascal999/torc``
2. Run ``docker run -i -t -p 127.0.0.1:5000:5000 -p 127.0.0.1:8080:8080 rascal999/torc torc.sh``
3. Visit http://127.0.0.1:8080/ for the torc-web client

#### From the Python Package Index (for development)

1. Execute ``pip install torc``

#### From this repository

1. Clone the Git repository
2. Change into the newly created directory
3. Execute ``pip install .``

## Usage

Running torc will start the web server.

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Credits

Developed by Aidan Marlin (aidan [dot] marlin [at] gmail [dot] com).
