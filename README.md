# <img src="https://www.holbertonschool.com/assets/holberton-logo-simplified-71b02868461c07d54553e4a7cc05d1926681a6755cc19030b0458f2d70ae9909.png" width="30"> AirBnB Clone V.4 - Web dynamic

## Synopsis
This is the 4rd version of our AirBnB clone project. We will be using a RESTful API, Flask, and jQuery AJAX

<p><img src="https://s3.amazonaws.com/intranet-projects-files/concepts/74/hbnb_step5.png" alt="step2"></p>

## Table of Contents
* [Environment](#environment)
* [Installation](#installation)
* [File Descriptions](#file-descriptions)
* [Usage](#usage)
* [Examples of use](#examples-of-use)
* [Bugs](#bugs)
* [Authors](#authors)
* [License](#license)

## Environment
This project is interpreted/tested on Ubuntu 14.04 LTS using python3 (version 3.4.3), jQuery (version 3.x), MySQL (version 5.7), Flask, and Chrome (version 57.0)

## Installation
** UNDER CONSTRUCTION **

## File Structure
[0-setup_web_static.sh](0-setup_web_static.sh) - bash script that sets up web servers for the deployment of `web_static`

[1-pack_web_static.py](1-pack_web_static.py) - Fabric script that generates a .tgz archive from the contents of `web_static`, using the function `do_pack`

[2-do_deploy_web_static.py](2-do_deploy_web_static.py) - Fabric script (based on [1-pack_web_static.py](1-pack_web_static.py)) that distributes an archive to web servers, using the function `do_deploy`

[3-deploy_web_static.py](3-deploy_web_static.py) - Fabric script (based on [2-do_deploy_web_static.py](2-do_deploy_web_static.py)) that creates and distributes an archive to web servers, using the function `deploy`

[AUTHORS](AUTHORS) - list of Authors who have worked on this project.

[console.py](console.py) - the console is a command line used to interact with the storage engines. 

[setup_mysql_dev.sql](setup_mysql_dev.sql) - MySQL script to set-up the hbnb_dev_db database.

[setup_mysql_test.sql](setup_mysql_test.sql) - MySQL script to set-up the hbnb_test_db database.

### [/models/](/models) directory contains all classes used for this project:
[base_model.py](/models/base_model.py) - The BaseModel class from which future classes will be derived

Classes inherited from Base Model:
* [amenity.py](/models/amenity.py)
* [city.py](/models/city.py)
* [place.py](/models/place.py)
* [review.py](/models/review.py)
* [state.py](/models/state.py)
* [user.py](/models/user.py)

#### [/models/engine/](/models/engine) directory contains all storage classes:
[file_storage.py](/models/engine/file_storage.py) - serializes/deserializes instances to/from a JSON file
[db_storage.py](/models/engine/db_storage.py) - saves and loads instances to/from a MySQL database

### [/tests/](/tests) directory contains all unit test cases for this project:
[/test/test_console.py](/test/test_console.py) - tests the console's functionality, documentation, and style

#### [/tests/models/](/tests/models) directory contains the unit tests for all classes:
[/test_models/test_base_model.py](/tests/test_models/test_base_model.py) - tests the BaseModel class' functionality, documentation, and style

[/test_models/test_amenity.py](/tests/test_models/test_amenity.py) - tests the Amenity class' functionality, documentation, and style

[/test_models/test_city.py](/tests/test_models/test_city.py) -tests the City class' functionality, documentation, and style

[/test_models/test_place.py](/tests/test_models/test_place.py) - tests the Place class' functionality, documentation, and style

[/test_models/test_review.py](/tests/test_models/test_review.py) - tests the Review class' functionality, documentation, and style

[/test_models/state.py](/tests/test_models/test_state.py) - tests the State class' functionality, documentation, and style

[/test_models/user.py](/tests/test_models/test_user.py) - tests the User class' functionality, documentation, and style

##### [/tests/models/engine/](/tests/models/engine) directory contains the unit tests for all storage classes:

[/test_models/test_file_storage.py](/tests/test_models/test_file_storage.py) - tests the FileStorage class' functionality, documentation, and style

[/test_models/test_db_storage.py](/tests/test_models/test_db_storage.py) - tests the DBStorage class' functionality, documentation, and style

### [/web_static/](/web_static) directory contains all html, css and images used for the static website.
[/web_static/8-index.html](8-index.html) - last iteration of static html.

#### [/web_static/styles/](/web_static/styles) directory contains all css used for the static website.
[/web_static/styles/3-footer.css](/web_static/styles/3-footer.css) - last iteration of css for the footer.

[/web_static/styles/3-header.css](/web_static/styles/3-fheader.css) - last iteration of css for the header.

[/web_static/styles/4-common.css](/web_static/styles/4-common.css) - last iteration of css for the body.

[/web_static/styles/6-filters.css](/web_static/styles/6-filters.css) - last iteration of css for the filters.

[/web_static/styles/8-places.css](/web_static/styles/8-places.css) - last iteration of css for the places display.

#### [/web_static/images](/web_static/images) contains all images used for the static website.
[/web_static/images/icon.png](/web_static/images/icon.png) - HBnB icon.

[/web_static/images/icon_bath.png](/web_static/images/icon_bath.png) - icon of a bath.

[/web_static/images/icon_bed.png](/web_static/images/icon_bed.png) - icon of a bed.

[/web_static/images/icon_group.png](/web_static/images/icon_group.png) - icon of a group of people.

[/web_static/images/logo.png](/web_static/images/logo.png) - HBnB logo.

### [/web_flask/](/web_flask) directory contains all files necessary to start a Flask web application.
[/web_static/100-hbnb.py](100-hbnb.py) - last iteration of flask application.

#### [/web_flask/static/](/web_static/styles) directory contains all images and css used for the Flask web application.

##### [/web_flask/static/styles](/web_static/styles) directory contains all css used for the Flask web application.
[/web_static/styles/3-footer.css](/web_static/styles/3-footer.css) - last iteration of css for the footer.

[/web_static/styles/3-header.css](/web_static/styles/3-fheader.css) - last iteration of css for the header.

[/web_static/styles/4-common.css](/web_static/styles/4-common.css) - last iteration of css for the body.

[/web_static/styles/6-filters.css](/web_static/styles/6-filters.css) - last iteration of css for the filters.

[/web_static/styles/8-places.css](/web_static/styles/8-places.css) - last iteration of css for the places display.

##### [/web_flask/static/images](/web_static/images) contains all images used for the Flask web application.
[/web_flask/static/images/icon.png](/web_flask/static/images/icon.png) - HBnB icon.

[/web_flask/static/images/icon_bath.png](/web_flask/static/images/icon_bath.png) - icon of a bath.

[/web_flask/static/images/icon_bed.png](/web_flask/static/images/icon_bed.png) - icon of a bed.

[/web_flask/static/images/icon_group.png](/web_flask/static/images/icon_group.png) - icon of a group of people.

[/web_flask/static/images/logo.png](/web_flask/static/images/logo.png) - HBnB logo.


## Examples of use
```
vagrantAirBnB_clone$./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  all  create  destroy  help  quit  show  update

(hbnb) all MyModel
** class doesn't exist **
(hbnb) create BaseModel
7da56403-cc45-4f1c-ad32-bfafeb2bb050
(hbnb) all BaseModel
[[BaseModel] (7da56403-cc45-4f1c-ad32-bfafeb2bb050) {'updated_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772167), 'id': '7da56403-cc45-4f1c-ad32-bfafeb2bb050', 'created_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772123)}]
(hbnb) show BaseModel 7da56403-cc45-4f1c-ad32-bfafeb2bb050
[BaseModel] (7da56403-cc45-4f1c-ad32-bfafeb2bb050) {'updated_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772167), 'id': '7da56403-cc45-4f1c-ad32-bfafeb2bb050', 'created_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772123)}
(hbnb) destroy BaseModel 7da56403-cc45-4f1c-ad32-bfafeb2bb050
(hbnb) show BaseModel 7da56403-cc45-4f1c-ad32-bfafeb2bb050
** no instance found **
(hbnb) quit
```

## Bugs
No known bugs at this time.

## Authors

###### Version 4

- Alexa Orrico - [Github](https://github.com/alexaorrico) / [Twitter](https://twitter.com/alexa_orrico)  
- Thomas Wang - [Github](https://github.com/thomaspwang) / [Twitter](https://twitter.com/thpwang)

###### Version 3

- Alexa Orrico - [Github](https://github.com/alexaorrico) / [Twitter](https://twitter.com/alexa_orrico)  
- Felicia Hsieh - [Github](https://github.com/feliciahsieh) / [Twitter](https://twitter.com/feliciahsiehsw)

###### Version 2

- Andrew Birnberg - [Github](https://github.com/birnbera) / [Twitter](https://twitter.com/birnbera)
- Thomas Wang - [Github](https://github.com/thomaspwang) / [Twitter](https://twitter.com/thpwang)

###### Version 1

- Alexa Orrico - [Github](https://github.com/alexaorrico) / [Twitter](https://twitter.com/alexa_orrico)  
- Jennifer Huang - [Github](https://github.com/jhuang10123) / [Twitter](https://twitter.com/earthtojhuang)

## License
Public Domain. No copywrite protection.
