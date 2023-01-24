## Project description
- Created integration tests in Postman based on a simple store template
- Added GitHub action to run `petstore.collection.json` in Github pages

## Technologies
- Node.js: 16.14.2
- Newman: 5.3.2,
- newman-reporter-htmlextra: 1.22.11
- Postman: 10.8.0

## Project set up
1. Clone the project `git clone https://github.com/PZhannet/-Postman-newman-ghActions`
2. Move to the Postman_API_testing folder `cd Postman_API_testing`
3. Run `npm i` (install node.js dependencies)

## Postman
 To run `store.collection.json`:
1. Run `npm run tern-on-api`(to run testing server locally )
2. Import file `store.collection.json` in Postman
3. Click the `Runner`
4. Drag one of the folders from the `store collection` into the `RUN ORDER` field
5. Press the `Run store` button
### store - Run results
![Run results](https://github.com/PZhannet/-Postman-newman-ghActions/blob/main/images/storeRunResults.png)

## Newman
- To run the collection through the command line
 `newman run {{name}}.collection.json`
- To create a new report in the ./docs directory 
 `newman run {{name}}.collection.json -r htmlextra --reporter-htmlextra-export docs/index.html`
- To run the `petstore.collection.json` through the command line and generate a report 
 `npm run run-report`

## GitHub Pages:
- To see generated HTML report with test execution `petstore.collection.json`:
- <a href="https://pzhannet.github.io/-Postman-newman-ghActions/"> Report </a>

### Newman Run Dashboard
![Newman Run Dashboard](https://github.com/PZhannet/-Postman-newman-ghActions/blob/main/images/newmanRunDashboard.png)
