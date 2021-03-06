# Sample Bitcoin RPC App

Study material for understanding various real scenarios and it's effect on the Bitcoin RPC usage.

Built by [Karl-Johan Alm](https://github.com/kallewoof) as training material for the [Blockchain Core Camp (BC2)](https://bc-2.jp/) workshop, this is for educational purposes only and not intended to be used in a production app.

## Getting Started

### Prerequisites

Make sure you have the following installed: 
* [Node.js](https://nodejs.org/en/)
* [MongoDB](https://www.mongodb.com/)
* [Mocha](http://mochajs.org/)

You can install those yourself, or follow these instructions.

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

### Installing

After downloading, copy the files into a folder inside your Bitcoin folder. Here, for example inside /rpcapp:

```
$ ls /<YOUR_BITCOIN_FOLDER>/rpcapp
api.js
bitcoin.js
[...]
```

From that folder, run `npm install` to get the necessary files:

```
$ cd /<YOUR_BITCOIN_FOLDER>/rpcapp
$ npm install
```

By default, this app uses `rpcuser=user` and `rpcpassword=password`, so either set those setting inside the [bitcoin.conf](https://en.bitcoin.it/wiki/Running_Bitcoin#Bitcoin.conf_Configuration_File) or change `config.js`.

If there are no issues, running ./rpc-cli should show something like this:

```
$ ./rpc-cli
available commands:
  create <amount> ...
  [...]
```

## Running the tests

Run npm test and work through the outputs:

```
$ npm test
```

## License

This project is licensed under the MIT License. See the [https://opensource.org/licenses/MIT](https://opensource.org/licenses/MIT) for more information.
