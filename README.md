
Real Estate Frontend Angular
Real Estate Application

Build Status

NPM version Linux Build Status Windows Build status Dependency Status devDependency Status Coverage Status

A website and user system, implemented with MongoDB, Express, AngularJS and Node.js, a.k.a MEAN stack. Inspired by and forked from Drywall.

Features

Versatility because you can
Hack your next awesome MEAN stack web app on top of Angular-Drywall, or
Use only the client as a non-trivial AngularJS project starter, or
Use only the sever as a pure User Management JSON API server.
Stand alone RESTful API service capable of serving any http clients, including iOS and Android app.
Social Login enabled currently for Facebook and Google.
Fully functional user life cycle management.
Admin panel provides full CRUD UI on all database entity.
Responsive web design supports Mobile-First Development.
Technology

Angular-Drywall's backend is pure Node.js RESTful API Server that renders no html pages . Front-end is built with AngularJS, Bootstrap and SASS. Grunt manages various development, testing and production build tasks.

On The Server	On The Client	Development
Express	AngularJS	Grunt
Mongo/Mongoose	Bootstrap	Npm
Passport	SASS	Bower
EmailJS	Font-Awesome	Karma
Moment.js	
Live demo

http://angular-drywall.arthurkao.io Hosted on AWS

Requirements

Have these packages installed and running on your system.

Node.js, and npm.
MongoDB
SASS
Grunt-cli
Bower
We use bcrypt for hashing secrets. If you have issues during installation related to bcrypt then refer to this wiki page.

Installation

$ git clone https://github.com/venkatreddyc/real-estate-app.git && cd ./real-estate-app
$ npm install
$ cd client && bower install && cd ..
Setup

Interactively setup basic website and necessary database configurations.

$ node init.js
Alternatively, modify config.example.js and initialize database manually. Not recommended.

$ cp ./config.example.js ./config.js
$ vi config.js  #set mongodb and email credentials
$ mongo # use mongo shell to insert required documents. Refer to ./init.js for the list of docs
Running the app

$ grunt

# > grunt

# Running "clean:src" (clean) task
# ...

# Running "concurrent:dev" (concurrent) task
# Running "watch" task
# Running "nodemon:dev" (nodemon) task
# Waiting...
# [nodemon] v1.2.1
# [nodemon] to restart at any time, enter `rs`
# [nodemon] watching: *.*
# [nodemon] starting `node app.js`
Now Angular-Drywall should be up and running at http://localhost:3000.

Login. Customize. Enjoy.

Philosophy

MEAN stack web app starter with user management up and running in 5 minutes.
Carefully built on top of latest state-of-the-art javascript technologies.
RESTful API service that easily serves non-browser (iOS, Android, among others) clients.
Single page web application.
Questions and contributing

Any issues or questions (no matter how basic), open an issue. Please take the initiative to include basic debugging information like operating system and relevant version details such as:

$ npm version

#{ 'angular-drywall': '0.1.1,
#  http_parser: '1.0',
#  node: '0.10.29',
#  v8: '3.14.5.9',
#  ares: '1.9.0-DEV',
#  uv: '0.10.27',
#  zlib: '1.2.3',
#  modules: '11',
#  openssl: '1.0.1h',
#  npm: '2.1.7' }
Contributions are welcome.

License

MIT
