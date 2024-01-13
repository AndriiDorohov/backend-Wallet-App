<p align="center">
    <a href="https://github.com/AndriiDorohov" target="_blank">
        <img src="https://github.com/AndriiDorohov/backend-Wallet-App/blob/main/images/project-logo.png" height="100px">
    </a>
    <h1 align="center">Yii 2 Basic Project Template</h1>
    <br>
</p>

# Wallet Backend

## _The Foundation of My Wallet Application_

[![Powered by Node.js, Express, and Swagger](https://img.shields.io/badge/Powered%20by-Node.js%2C%20Express%2C%20%26%20Swagger-%23339933)](https://github.com/AndriiDorohov/backend-Wallet-App)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Wallet Backend is a robust and secure server-side component that serves as the backbone for my
Wallet application. It provides a reliable foundation for managing user finances efficiently.

## DIRECTORY STRUCTURE

      db/                 contains database-related files
      docs/               contains project documentation
      logs.log            contains logs generated during runtime
      middlewares/        contains middleware files
      models/             contains model classes
      controllers/        contains controller classes
      routes/             contains route definitions
      utils/              contains utility files
      .env.example        example file for environment variables
      app.js              entry script for the application
      README.md           project documentation

## Features

- Import a HTML file and watch it magically convert to Markdown
- Drag and drop images (requires your Dropbox account be linked)
- Import and save files from GitHub, Dropbox, Google Drive and One Drive
- Drag and drop markdown and HTML files into Dillinger
- Export documents as Markdown, HTML and PDF

Markdown is a lightweight markup language based on the formatting conventions that people naturally
use in email. As [John Gruber] writes on the [Markdown site][df1]

> The overriding design goal for Markdown's formatting syntax is to make it as readable as possible.
> The idea is that a Markdown-formatted document should be publishable as-is, as plain text, without
> looking like it's been marked up with tags or formatting instructions.

This text you see here is \*actually- written in Markdown! To get a feel for Markdown's syntax, type
some text into the left window and watch the results in the right.

## Tech

The "Wallet Backend" project leverages a variety of open-source technologies:

- [Node.js] - event-driven I/O for the backend
- [Express] - fast framework for building network applications on Node.js
- [Swagger] - tool for creating interactive API documentation
- [Mongoose] - library for modeling objects for MongoDB and Node.js
- [Axios] - HTTP client for making requests
- [Cors] - package for handling CORS requests in Express
- [jsonwebtoken] - library for generating and verifying JWT tokens
- [bcryptjs] - library for hashing passwords
- [dotenv] - module for loading environment variables from a .env file
- [log4js] - library for event logging in Node.js
- [moment] - library for working with dates and times in JavaScript
- [uuid] - generator for unique identifiers
- [validator] - library for data validation

And, of course, the "Wallet Backend" itself is an open-source project with a public repository on
GitHub.

## Installation

For running the "Wallet Backend," you need [Node.js](https://nodejs.org/) v12+ installed on your
system.

Clone the repository

```sh
git clone https://github.com/AndriiDorohov/backend-Wallet-App.git
```

Navigate to the project directory

```sh
cd backend-Wallet-App
```

Install dependencies

```sh
npm install
```

Start the development server

```sh
npm run start:dev
```

##### For production environments

Install production dependencies

```sh
npm install --production
```

Set the environment to production and start the server

```sh
NODE_ENV=production npm start
```

## Development

Want to contribute? Great!

Dillinger uses Gulp + Webpack for fast developing. Make a change in your file and instantaneously
see your updates!

Open your favorite Terminal and run these commands.

First Tab:

```sh
node app
```

Second Tab:

```sh
gulp watch
```

(optional) Third:

```sh
karma test
```

#### Building for source

For production release:

```sh
gulp build --prod
```

Generating pre-built zip archives for distribution:

```sh
gulp build dist --prod
```

## Docker

Dillinger is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 8080, so change this within the Dockerfile if necessary.
When ready, simply use the Dockerfile to build the image.

```sh
cd dillinger
docker build -t <youruser>/dillinger:${package.json.version} .
```

This will create the dillinger image and pull in the necessary dependencies. Be sure to swap out
`${package.json.version}` with the actual version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on your host. In this example,
we simply map port 8000 of the host to port 8080 of the Docker (or whatever port was exposed in the
Dockerfile):

```sh
docker run -d -p 8000:8080 --restart=always --cap-add=SYS_ADMIN --name=dillinger <youruser>/dillinger:${package.json.version}
```

> Note: `--capt-add=SYS-ADMIN` is required for PDF rendering.

Verify the deployment by navigating to your server address in your preferred browser.

```sh
127.0.0.1:8000
```

## License

MIT

**Free Software, Hell Yeah!**

[//]:
  #
  "These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax"
[dill]: https://github.com/joemccann/dillinger
[git-repo-url]: https://github.com/joemccann/dillinger.git
[john gruber]: http://daringfireball.net
[df1]: http://daringfireball.net/projects/markdown/
[markdown-it]: https://github.com/markdown-it/markdown-it
[Ace Editor]: http://ace.ajax.org
[node.js]: http://nodejs.org
[Twitter Bootstrap]: http://twitter.github.com/bootstrap/
[jQuery]: http://jquery.com
[@tjholowaychuk]: http://twitter.com/tjholowaychuk
[express]: http://expressjs.com
[AngularJS]: http://angularjs.org
[Gulp]: http://gulpjs.com
[PlDb]: https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md
[PlGh]: https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md
[PlGd]: https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md
[PlOd]: https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md
[PlMe]: https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md
[PlGa]: https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md
