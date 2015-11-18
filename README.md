# Restaurants

This is a fully educational server-side solution based on free course materials at Udacity platform. Provided Python code is able to create a database and display restaurants with menus at a simple, editable website.

## Installation

#### Server Dependencies

- Python 2.7
- SQLAlchemy
- Flask framework

For development, [Virtual Box](https://www.virtualbox.org/wiki/Downloads) and a configured [Vagrant](https://www.vagrantup.com/downloads) server running [Ubuntu](https://github.com/ludgo/Restaurants/blob/master/Vagrantfile) were used (see [configuration file](https://github.com/ludgo/Restaurants/blob/master/pg_config.sh)).

#### Launch

Assuming that the server is running:

1. create a SQLite [database](https://github.com/ludgo/Restaurants/blob/master/Restaurants/database_setup.py)
2. [fill](https://github.com/ludgo/Restaurants/blob/master/Restaurants/database_fill.py) the database with dummy data
3. [launch](https://github.com/ludgo/Restaurants/blob/master/Restaurants/backend_restaurants.py) the website at specified port

## Functionality

Users basically can:

- Browse restaurants and their menus following responsive design
- Manage direcly all the persistent data storage (CRUD functions)
- Take advantage of Google Street View Image API up to image size 640px x 640px

JSON API with both restaurant list and menu items was implemented. It can be accessed by appending **json** query parameter either to root URL or parameterized URL:

- `<base-url>/json` to get information about restaurants
- `<base-url>/restaurant/<restaurant-id>/json` to get information about menu at the particular restaurant

<br/>
<br/>

![Alt text](https://github.com/ludgo/Restaurants/blob/master/teaser1.jpg)

![Alt text](https://github.com/ludgo/Restaurants/blob/master/teaser2.jpg)

## Acknowledgments

Special thanks to Udacity for providing free access to the course materials including both front-end and back-end web technologies.
