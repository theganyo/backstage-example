# backstage-example

This repository contains an example [Backstage](https://backstage.io) developer
portal application for browsing data exported from API Hub.

## API Hub Data

API Hub data for Backstage is maintained in
[backstage-export](https://github.com/apigee-apihub-demo/backstage-export) repo.
This data is automatically read by the Backstage demo in this repo.

## Running Backstage

### Docker

The easiest way to run is by using the published docker image. Example:

```sh
docker run -p 7007:7007 ghcr.io/apigee-apihub-demo/backstage-example:main
```

Then, open the application on your web browser at http://localhost:7070.

### Development

#### Running

To do local development on Backstage, be sure you've installed the
[prerequisites](https://backstage.io/docs/getting-started/#prerequisites) then
[run using yarn](https://backstage.io/docs/getting-started/#run-the-backstage-app):

```sh
cd apigee-apihub-demo; yarn dev
```

Once running, your default browser should open automatically to the application
at http://localhost:3000.

#### Updating Backstage

Follow the advice of the
[Backstage docs](https://backstage.io/docs/getting-started/keeping-backstage-updated):

```sh
yarn backstage-cli versions:bump
```

## Disclaimer

This demonstration is not an officially supported Google product.

## License

Unless otherwise specified, all content is owned by Google, LLC and released
with the Apache license.
