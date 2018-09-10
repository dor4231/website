# PositiveYou - The Website

## Description

At first, the main porpus of this site is to attract potential customers and make them understand why we are the best company to work with.

Secondly, our members who already works with us can find update about the progress of thier project and easily find someone to support them if somthing went wrong.

## Installation

Read about the structure to get deeper understanding about what you are doing in this section.

1. git clone this repository.

2. Create virtual environment using python 3.6 and call it `venv` in order for git to ignore it (Use this for the [full virtualenv guid](https://virtualenv.pypa.io/en/stable/userguide/)).

3. Activate the virtualenv (macOS: `source venv/bin/activate` ; Windows: `./venv/Scripts/activate.bat`).

4. Install python requerments: `python -m pip install -r requirements.txt`.

5. Install `gulp` and `gulp-cli` using this commands: `npm install gulp` and `npm install -g gulp-cli`. [Read more about Gulp](https://gulpjs.com/)

6. `cd` into the `positiveyou-react` folder.

7. Install all npm dependencies. Run command: `npm install`.

## Run the server

### Django serve everythig

You should build the Front-End app and copy it into the correct place (use the gulp `build` task for that).

1. `cd` into the `positiveyou-react` folder

2. Run command `npm run build`.

3. Navigate into the root folder of the project: `cd ..`.

4. Run the gulp build task: `gulp react-to-django`

5. `cd` into `positiveyou` folder.

6. Run the django server: `python manage.py runserver` and open the `localhost` link in the browser using the given port.

### Django and React development servers

You should run both servers as standalone servers and make them to comunicate.

1. Run the Django server. Make sure you are in the `positiveyou` folder and run `python manage.py runserver`.

2. Run the React server.  Make sure you are in the `positiveyou-react` folder and run `npm start`.

3. Make sure cross-origin is anabled in the Django server.

4. Make sure the api calls from the React app send it's requests to the correct URL (The URL provided by the Django server).

## Structur

This project is built with Django and React. Django has an app named Frontend that holds the build of the React project. The rest of the apps in the Django project are for hadnling API call the Front End app makes.

The React project is an SPA, all the functionality of the backend is ececuted through this application.

## Contribute

If you find this project interresting, you like the vibe of our team or we just look like nice people feel free to tell us and join the team.

This is not a standart open source project, it's the hart of our company - Open and free to use, copy and modifi.

## Secret Keys

All secret key are not included in this repository. There is a template for all secrets called secret-settings.py.template.

Simply rename it to secret-settings.py and set some proper keys for each value as needed to make the whole app work.
