<<<<<<< HEAD
# Hello SQLite!

This project includes a [Node.js](https://nodejs.org/en/about/) server script that uses a persistent [SQLite](https://www.sqlite.org) database. The app also includes a front-end with two web pages that connect to the database using the server API. 📊

The home page presents the user with a poll where they can choose an option, then the page presents the results in a chart. The admin page displays the log of past choices and allows the user to clear it by supplying an admin key (you can set this up by following the steps in `TODO.md`). 🔒

_Last updated: 14 August 2023_

## Prerequisites

To get best use out of this project you'll ideally be familiar with JavaScript and have a little Node.js experience–check out [Hello Node](https://glitch.com/~glitch-hello-node) if you haven't already!

=======
# Hello React! (blank)

[React](https://reactjs.org/) is a popular UI library for building web apps, usually single page apps. [Vite](https://vitejs.dev/) is a powerful tool for building javascript apps that bundles all of your code and shows immediate changes while you're editing. We're big fans!

While you're in the editor working, Glitch is running your `start` script in the background (`vite dev`). The site will be in dev mode and you'll see your changes happen 🪄 immediately in the preview window. Once you close the editor window and your app goes to sleep, Glitch runs the `build` script and Vite builds your app for modern browsers.

_Last updated: 14 August 2023_

>>>>>>> 01_mybranch
## What's in this project?

← `README.md`: That’s this file, where you can tell people what your cool website does and how you built it.

<<<<<<< HEAD
← `package.json`: The NPM packages for your project's dependencies.

← `.env`: The environment is cleared when you initially remix the project, but you will add a new env variable value when you follow the steps in `TODO.md` to set up an admin key.

### Server and database

← `server.js`: The Node.js server script for your new site. The JavaScript defines the endpoints in the site API. The API processes requests, connects to the database using the `sqlite` script in `src`, and sends info back to the client (the web pages that make up the app user interface, built using the Handlebars templates in `src/pages`).

← `/src/sqlite.js`: The database script handles setting up and connecting to the SQLite database. The `server.js` API endpoints call the functions in the database script to manage the data.

← `/src/data.json`: The data config file includes the database manager script–`server.js` reads the `database` property to import the correct script.

When the app runs, the scripts build the database:

← `.data/choices.db`: Your database is created and placed in the `.data` folder, a hidden directory whose contents aren’t copied when a project is remixed. You can see the contents of `.data` in the console by selecting __Tools__ >  __Logs__.

### User interface

← `public/style.css`: The style rules that define the site appearance.

← `src/pages`: The handlebars files that make up the site user interface. The API in `server.js` sends data to these templates to include in the HTML.

← `src/pages/index.hbs`: The site homepage presents a form when the user first visits. When the visitor submits a preference through the form, the app calls the `POST` endpoint `/`, passing the user selection. The `server.js` endpoint updates the database and returns the user choices submitted so far, which the page presents in a chart (using [Chart.js](https://www.chartjs.org/docs/)–you can see the code in the page `head`).

← `src/pages/admin.hbs`: The admin page presents a table displaying the log of most recent picks. You can clear the list by setting up your admin key (see `TODO.md`). If the user attempts to clear the list without a valid key, the page will present the log again.

← `src/seo.json`: When you're ready to share your new site or add a custom domain, change SEO/meta settings in here.

## Try this next 🏗️

Take a look in `TODO.md` for steps in setting up your admin key and adding to the site functionality.

💡 __Want to use the server script as an API without using the front-end UI? No problem! Just send a query parameter `?raw=json` with your requests to return JSON, like this (replace the first part of the URL to match your remix): `glitch-hello-sqlite.glitch.me?raw=json`__

___Check out [Blank SQLite](https://glitch.com/~glitch-blank-sqlite) for a minimal demo of get, post, put, and delete methods.___
=======
← `index.html`: This is the main page template React uses to build your site. When you're ready to share it or add a custom domain, change SEO/meta settings in here.

← `src/`: This folder contains all the files React will use to build your site.

### Working in the `src/` folder 📁

← `src/index.jsx`: This is the root of your React app. If you add libraries like [chakra-ui](https://chakra-ui.com) or [redux](https://react-redux.js.org), you'll insert their providers here. The `<HelmetProvider`> is an example of a provider you'd use.

← `src/app.jsx`: The base for your react app, here is where the magic really happens.

← `src/pages/`: Pages to import to the router should go here!

← `src/styles`: CSS files add styling rules to your content. You have [a lot of](https://vitejs.dev/guide/features.html#css) importing options for CSS including CSS modules if that's your jam.
>>>>>>> 01_mybranch

![Glitch](https://cdn.glitch.com/a9975ea6-8949-4bab-addb-8a95021dc2da%2FLogo_Color.svg?v=1602781328576)

## You built this with Glitch!

[Glitch](https://glitch.com) is a friendly community where millions of people come together to build web apps and websites.

<<<<<<< HEAD
=======
- Want more details about React on Glitch? We've got a [Help Center article](https://help.glitch.com/hc/en-us/articles/16287545215501-React-Projects) for you.
>>>>>>> 01_mybranch
- Need more help? [Check out our Help Center](https://help.glitch.com/) for answers to any common questions.
- Ready to make it official? [Become a paid Glitch member](https://glitch.com/pricing) to boost your app with private sharing, more storage and memory, domains and more.
