here i write notes that i will take during the progres of making this app

# front end

1. we change the folder structere in te nuxt project
   we do inteed use Pages :)

2. pages/index.vue
   this is youre home page, for example we add all the components on here

3. componets/search.vue
   ref('') stores reactive input data
   v-model conects the input to Vue state
   boostrap for styling

   what does component search.vue
   1. Create reactive variables (location, weather, loading, error)
   2. create a function to fecht weather data
   3. reset state before feching
   4. validate input (location must not be empty) 5. show loading state
   5. call backend api
   6. save results in weather
   7. handle errors if request fails
   8. stop loading
      10.Rendering UI (input, buttons, messages, weather data)

# back end

understand the important Symfony folders

src/
Your PHP application code lives here

src/Controller/
Controllers receive HTTP request and return responses

config/
framework configuration

routes/
Route definitions if you use rout files, though maney Symfony apps define routes with PHP attributes in controllers.

.env
Envirometn variables for local development

1. install Symfony HTTP client: composer require symfony/http-client
   Youre back end needs to call the external weather API
   Symfony's HTTP client is the normal clean way to make outgoing request

2. what does WeatherController
   1. wait for GET api/weather
   2. Read the location from current query string // import HTTPFoundation!!!
      checks if the current data exist
      if no location, return 400 error
   3. Read API key form .env
   4. if no APIkey then show 500 error
   5. Build weather API URL
   6. call external API
   7. Retrun JSON back to the front end

   what are the main blocks
   1. namespaces and imports
   2. controller clas
   3. route defenitions
   4. method parameters
   5. imput validation
   6. API key check
   7. URL building
   8. API call.
   9. JSON Response
   10. error handeling

URL to test if controller is working: https://localhost:8000/api/weather?location=Amsterdam
