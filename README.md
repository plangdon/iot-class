# Commercial IoT Class

## Installing on your hardware - some scripts

### Using Intel NUC Gateways
- [NUC Gateway Setup](gateway-setup/README.md)

### Using Raspberry Pi
- [Raspberry Pi Setup](raspi/README.md)

### Or follow instructions for your specific platform at [https://nodered.org/](https://nodered.org/)

## Examples and Flow Libraries
- Intel IoT Gateway - [https://github.com/intel-iot-devkit/Intel-IoT-Gateway]
- Library at node-red.org - [https://flows.nodered.org/]
- IBM Node-red Labs (https://github.com/jeancarl/node-red-labs)

### In this repo
- IP Address to LCD - [node-red-examples/ip-to-lcd/README.md](node-red-examples/ip-to-lcd/README.md)
- Simple Webserver - [node-red-examples/simple-webserver/README.md](node-red-examples/simple-webserver/README.md)
- MQTT - [node-red-examples/mqtt/README.md](node-red-examples/mqtt/README.md)
- Websockets - [node-red-examples/websockets/README.md](node-red-examples/websockets/README.md)

## Adding nodes

Node-RED comes with a core set of useful nodes, but there are a growing number of additional nodes available for install from both the Node-RED project as well as the wider community.

You can search for available nodes in the [Node-RED library](http://flows.nodered.org/) or on the [npm repository](https://www.npmjs.com/browse/keyword/node-red).

### Using the Editor

From version 0.15 you can install nodes directly using the editor. To to this select **Manage Palette** from the menu (top right), and then select the **install** tab in the palette. You can now search for new nodes to install, and enable and disable existing nodes.

### Installing npm packaged nodes###

To install an npm-packaged node, you can either install it locally within your user data directory (by default, $HOME/.node-red):

`cd $HOME/.node-red`
`npm install <npm-package-name>`
or globally alongside Node-RED:

`sudo npm install -g <npm-package-name>`
You will need to restart Node-RED for it to pick-up the new nodes.

Installing individual node files

It is also possible to install nodes by copying their .js and .html files into a nodes directory within your user data directory. If these nodes have any npm dependencies, they must be also be installed within the user data directory. This is only really recommended for development purposes.

