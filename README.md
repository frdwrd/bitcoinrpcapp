# Sample Bitcoin RPC App

Originally built as training material for the [Blockchain Core Camp (BC2)](https://bc-2.jp/) workshop. 

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

### Installing

Copy the files into a folder inside your Bitcoin folder. For example /rpcapp

```
$ mkdir /<YOUR_BITCOIN_FOLDER>/rpcapp
$ cd /<YOUR_BITCOIN_FOLDER>/rpcapp
$ git clone https://github.com/dgarage/bitcoinrpcapp
```

Make sure you have Node.js, MongoDB, and Mocha installed.

For OSX (assuming you have Homebrew installed):

```
$ brew install node mongodb
$ brew services start mongodb
$ npm install -g mocha #sometimes this might require sudo
```

For Ubuntu 64-bit:

```
$ sudo apt-get install curl
$ curl -sL https://deb.nodesource.com/setup_7.x | sudo -E bash -
$ sudo apt-get install nodejs mongodb
$ sudo systemctl start mongodb
$ sudo systemctl enable mongodb
$ sudo ln -s /usr/bin/nodejs /usr/local/bin/node # nodeがないとバグったりする
$ sudo npm install -g mocha
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management

## License

This project is licensed under the MIT License. See the [https://opensource.org/licenses/MIT](https://opensource.org/licenses/MIT) for more information.