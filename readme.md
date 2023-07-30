# Project: Single Page Application: Javascript, HTML, CSS

- General project requirements here: https://github.com/learn-co-curriculum/phase-1-javascript-project-mode

# The basic story of the application
  - A Single Page Application (SPO) that allows the user to get and generate memes. Receives a list of memes, can generate one, can like memes, and then add memes to the database and as a result the website. Add their email to an email list, and there is some "easter-egg" functionality as well.
  
# Running the local server, authentication
- json-server --watch db.json
- explorer.exe index.html
- store api key in .env file of format (note that this is .gitignored) # TODO UPDATE

# Requires and API key (follow instructions here as needed)
- http://apimeme.com/?ref=apilist.fun
- https://rapidapi.com/meme-generator-api-meme-generator-api-default/api/meme-generator

### Project Objective, Plan, Features & User Stories

### Project Plan

- **The basic story of your application**
  - A Single Page Application (SPO) that allows the user to get and generate memes. Receives a list of memes, can generate one, can like memes, and then add memes to the database and as a result the website. Add their email to an email list, and there is some "easter-egg" functionality as well.

- **Core features of your MVP**
  - Upon SPA loading, see all the previously made memes by other users. 
  - Ability to "like" any of the displayed memes. Persists in the database.
  - Drop-down filter "list of memes" that can be used to generate a new meme.
  - Generate meme button with user input for text at top and bottom of image.
  - Returns the generated image with user text. 
  - Adds the returned meme to the persistant data storage.
  - User can add their email to an email list, and gets a "surprise".

- **API, Data, And Use**
  - https://rapidapi.com/meme-generator-api-meme-generator-api-default/api/meme-generator
  - Using the getImages/ endpoint to get a list of all images avaiable from the API.
  - Using the generateMeme/ endpoint to get a JSON image from the API.
  - Local json-server database GET, POST and PATCH.

- **Challenges you expect to face.**
  - Persisting images without a true backend database.
  - Protecting sensitive information.
  - Scope creep.

**User Stories and API Interation**

  - **User Stories**
  - "As a new user, I want to be able to see a list of memes I can use".
  - "As a influencer, I want to be able to make memes with text, so I can get lots of likes and laughs".
  - "As a bored user, I want to be able to see memes other people have made".
  - "As a creative user, I want to have my meme on the website for others to see." 

- **API Interation & structure**
  - GET request to meme API for all available memes.
  - GET request to meme generator API to generate a meme.
  - GET request to local json database to show all existing memes already created.
  - POST request to local json database to add new meme (new record, update likes).

# Resources
- https://rapidapi.com/guides/fetch-images-with-fetch-api
- https://rapidapi.com/meme-generator-api-meme-generator-api-default/api/meme-generator
- https://www.w3docs.com/learn-html/html-select-tag.html
- https://www.youtube.com/watch?v=cP5E0b21f_Y
- https://open-code.tech/en/post-1424/
- https://stackoverflow.com/questions/21518381/
- proper-way-to-wait-for-one-function-to-finish-before-continuing
- https://www.freecodecamp.org/news/gitignore-file-how-to-ignore-files-and-folders-in-git/#ignore-file
- https://stackoverflow.com/questions/5786851/define-a-global-variable-in-a-javascript-function