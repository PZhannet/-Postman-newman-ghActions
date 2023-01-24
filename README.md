## Project description
- Created integration tests in Postman based on a simple store template
- Added GitHub action to run `petstore.collection.json` in Github pages

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
<p align="center">
  <img src="./images/storeRunResults.png" width="350" title="hover text">
</p>

## Newman
- To run the collection through the command line
 `newman run {{name}}.collection.json`
- To create a new report in the ./docs directory 
 `newman run {{name}}.collection.json -r htmlextra --reporter-htmlextra-export docs/index.html`
- To run the `petstore.collection.json` through the command line and generate a report 
 `npm run run-report`

## GitHub Pages:
- To see generated HTML report with test execution `petstore.collection.json`:
    <a href="https://pzhannet.github.io/-Postman-newman-ghActions/"> Report </a>

### Newman Run Dashboard
![Newman Run Dashboard](https://pzhannet.github.io/-Postman-newman-ghActions/)
