# Getting Started

Welcome to your new project.

It contains these folders and files, following our recommended project layout:

File or Folder | Purpose
---------|----------
`app/` | content for UI frontends goes here
`db/` | your domain models and data go here
`srv/` | your service models and code go here
`package.json` | project metadata and configuration
`readme.md` | this getting started guide


## Next Steps

- Open a new terminal and run `cds watch` 
- (in VS Code simply choose _**Terminal** > Run Task > cds watch_)
- Start adding content, for example, a [db/schema.cds](db/schema.cds).


## Learn More

Learn more at https://cap.cloud.sap/docs/get-started/.

## Package to add
npm i @sap-cloud-sdk/resilience

npm i @sap-cloud-sdk/http-client
npm i hdb
npm i @sap/hana-client
npm i @sap/hdi
npm i@sap/hdi-deploy

## To add HANA cloud for Production
cds add hana --for production

## To add XSUAA for prod
cds add xsuaa --for production

## To Generate the xs-security
cds compile srv/ --to xsuaa > xs-security.json

## Create the MTA descriptor file for MTA-Based deployment.
cds add mta

## To Add the managed approuter as gateway to the project.
cds add approuter --for production