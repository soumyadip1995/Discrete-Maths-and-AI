## Discrete-Maths-and-AI


A study of transit system design using graph theory.

## Frontend

Network Analysis: [https://gtfs-graph.herokuapp.com/](https://gtfs-graph.herokuapp.com/)
* Page Rank
* Closeness Centrality
* Katz Centrality
* Accessibility
  * Reference: "Accessibility in complex networks", B.A.N. Travençolo and L. da Fontoura Costa, *Physics Letters A*, 2008.

Algorithm Demo: [https://gtfs-graph.herokuapp.com/demo/](https://gtfs-graph.herokuapp.com/demo/)
* Depth-First Search
* Breadth-First Search
* Dijkstra's Algorithm (Shortest Path Search)

## Usage

`gtfs-graph` requires Node.js version 7.2.1.

After cloning the repository, be sure to install the necessary dependencies.

`npm install`

There is an `npm` command to build the JavaScript bundle and start the Node.js server. These are not joined because the combine sequence takes longer than 60 seconds to complete, with is Heroku's limit on server boot time. See Other for the component commands.

`npm run all`

### Test

A test suite of mostly unit tests is included. To run the tests:

`npm test`

### Other

To build the JavaScript bundle without starting the server, run:

`npm run build-js`

Then, the Node.js server may be started.

`npm start`

### Advanced Usage

Command-line options are available for `lib/server/index.js` to customize a run.

`--system` will load the server for only a single specified system. Default: all.

`node lib/server/index.js --system MBTA`

`--verbosity` will run the server at the specified verbosity. Default: info.

`node lib/server/index.js --verbosity verbose`
