#FFW Styleguide Template

##Getting started

###Prerequisites:
The FFW Styleguide has a few dependencies that you will need to install to use it. Don't worry, we're got all the link you need right here:

* [Node.js](https://nodejs.org/en/) – The backbone of the framework. Node Package Manager takes care of installing all the dev dependencies,
* [Bower](http://bower.io/) – Bower manages all the front end packages and fetches them for, when we start a new project.
* [Gulp](http://gulpjs.com/) – Task manager and automation. Gulp is responsible for running all the small tasks like compiling SCSS and Twig templates, starting a web server and automatically reloading browsers.

###Starting a new project
So you got the prerequisites installed, and you're ready to get started? Great! Just follow the simple steps below:


1. Download a copy of the framework

2. Open up the project folder in Terminal.

3. Navigate to the .npm folder:

    ```
    cd .npm
    ```

4. Install all the required packages with Node Package Manager

    ```
    npm install
    ```
5. Install all the Bower packages:

    ```
    bower install
    ```

6. For just compile style:

    ```
    gulp sass-dev
    ```

7. Initialize the project with Gulp:

    ```
    gulp
    ```

## How to create a new component
1. Navigate to the `styleguide/components` folder
2. Create a new twig file: `component-name.twig`
3. Open file `data/global.json`, find array `list_components` then add this code into it

    ```
      {
        "id":"component-name", // Same as file name.
        "name": "Component Title"
      }
   ```

Make sure `gulp` is runing.