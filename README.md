The purpose of this repository is to provide a simple controllable API data to test SEO and react page rendering in different modes (SSR/SSG).

Live URL: https://fake-comic-api.herokuapp.com/

Running the application
```bash
git clone https://github.com/theFaruq/001-json-server.git

yarn install

yarn start
```

The default port is `8000` so the development URL is `http://localhost:8000`. 

Add a database/data-source

- Create a json file in the `data` directory, be sure to choose a good name because the file is used as your API path. Also make sure the file contains a valid JSON.
- Import and re-export the json file in `database.js` file.

Here's an example - say we want to create a database for zombies, given a `./data/zombie.json` file
```javascript
...
const zombie = require('./data/zombie');

module.exports = {
  ...
  zombie
}
```
NOTE: This is built on `json-server` package. Click [here](https://www.npmjs.com/package/json-server) to learn more about `json-server`.