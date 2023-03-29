
The structure of the project is:
- ```main.py``` the FastAPI main program the defines the routes.
- ```requirements.txt``` defines the required python packages for pip install.
- ```/static``` shows how to return "static files," i.e. HTML files.
  - ```/static/index.html``` a simple HTML file.
- ```tts``` some unit tests. I do not use something like "tests" because PyCharm thinks I want
to use some testing automation package. I would use automation in a larger project.
  - ```t_mysql_data_service``` unit tests MySQL interaction.
  - ```t_artist_resource``` unit tests the IMDB Artist resource for name_basics.
- ```/resources``` contains the implementation of the resources.
  - ```base_data_service``` is an abstract base class for access to databases.
  - ```mysql_data_service``` is an implementation of ```base_data_service``` foe MySQL.
  - ```base_application_resource``` is an abstract base class for REST resources.
  - ```/imdb_resources``` is implementation of IMDB specific resources.
    - ```/artist_resource``` implements the resource for name_basics.
