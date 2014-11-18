#Fake News
###Like Jon Stewart but better

These are the results of following the 'thinkster.io' tutorial at [this address](https://thinkster.io/angulartutorial/mean-stack-tutorial/ "Thinkster.io"). It provides a basic understanding of building a webapp in MEAN Stack ([MongoDB](http://www.mongodb.org/), [Express.js](http://expressjs.com/), [Angular.js](https://angularjs.org/), [Node.js](http://nodejs.org/)).

What you'll need to run the app:

1. Install [node.js](http://nodejs.org) on your local machine
2. Install [MongoDB](http://www.mongodb.org) on your local machine
3. `clone` the repo
4. `cd` into the working directory
5. Run `npm install` to get all the node_modules (you can look at the package.json file to see what modules are being installed.
6. Turn on MongoDB (`mongod`).
7. Run `npm start`
8. Go to `localhost:3000` on a browser (preferably Firefox or Chrome because IE sucks!).

#####How it works#####

######Data layer (Node, Express, MongoDB via Mongoose)######
* [Mongoose.js](http://mongoosejs.com/) is plugged into our Node app in order for us to facilitate communication with [MongoDB](http://mongodb.org) and model Schemas for Posts and Comments.
* We use [Express'](http://expressjs.com/) built-in router methods (GET, POST, PUT) to simulate a RESTful API interaction.
* Our Frontend uses [Angular's](http://angularjs.org) $http service to call the routes we created via [Express](http://expressjs.com/) to get the necessary data to render on the page as well as to let the user create new posts, create new comments and upvote (like) posts and comments. 