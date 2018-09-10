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
5. `cd` into the `positiveyou-react` folder.
6. Run command: `npm install`.


## Structur

This project is built with Django and React. Django has an app named Frontend that holds the build of the React project. The rest of the apps in the Django project are for hadnling API call the Front End app makes.

The React project is an SPA, all the functionality of the backend is ececuted through this application.



## Contribute

If you find this project interresting, you like the vibe of our team or we just look like nice people feel free to tell us and join the team.

This is not a standart open source project, it's the hart of our company - Open and free to use, copy and modifi.

## Secret Keys

All secret key are not included in this repository. There is a template for all secrets called secret-settings.py.template.

Simply rename it to secret-settings.py and set some proper keys for each value as needed to make the whole app work.
