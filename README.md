```
 _____                _    _ _         ____                                
|  ___| __ __ _ _ __ | | _| (_)_ __   |  _ \ ___  ___ _   _ _ __ ___   ___ 
| |_ | '__/ _` | '_ \| |/ / | | '_ \  | |_) / _ \/ __| | | | '_ ` _ \ / _ \
|  _|| | | (_| | | | |   <| | | | | | |  _ <  __/\__ \ |_| | | | | | |  __/
|_|  |_|  \__,_|_| |_|_|\_\_|_|_| |_| |_| \_\___||___/\__,_|_| |_| |_|\___|
                                                                           
```

[![Coverage Status](https://coveralls.io/repos/github/theDevilsVoice/franklin-resume/badge.svg?branch=master)](https://coveralls.io/github/theDevilsVoice/franklin-resume?branch=master)
[![Total alerts](https://img.shields.io/lgtm/alerts/g/theDevilsVoice/franklin-resume.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/theDevilsVoice/franklin-resume/alerts/)
[![Heroku](https://heroku-badge.herokuapp.com/?app=franklin-resume)

## Testing 

#### Run App on Localhost via Docker

- Type 'make local' to start the docker environment.
- Navigate to http://0.0.0.0:5000/

#### Create Docker Instance to Log in and Run `pytest`

- Type 'make local-dev' to build dev env. 
- Docker will setup up container and put you in the project directory. 
- Test like so:

```
make local-dev
pytest
py.test
tox -e pylint
tox -e venv
```

## Heroku

Log in to see what's up: 

```
heroku run bash --app franklin-resume
```

Tail the logs

```
heroku logs --tail -a franklin-resume
```

Heroku Releases

```
curl -n https://api.heroku.com/apps/franklin-resume/releases/ \
          -H "Accept: application/vnd.heroku+json; version=3"
```
