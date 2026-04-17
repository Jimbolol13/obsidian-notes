## front end

# first make frontend project(nuxt):

npx nuxi@latest init frontend

# second made backen project (symfony):

symfony new weather-backend --webapp

# install bootsrap

1. npm install bootstrap
2. add to 'nuxt.cnfig.ts' this: css: ["bootstrap/dist/css/bootstrap.min.css"],
3. in plugins/bootstrap.client.ts add: import "bootstrap/dist/js/bootstrap.bundle.min.js";

# next step

fill out index.vue
fill out component search

## back end

# add API key to .env

VISUAL_CROSSING_API_KEY="FXK2QBYTFFDZHUVXCR828RNAS"

# install Symfony HTTP client

composer require symfony/http-client

# generate controller:

php bin/console make:controller WeatherController
Then fill out the controller

# install CORS

composer require nelmio/cors-bundle
Location config file: config/packages/nelmio_cors.yaml
