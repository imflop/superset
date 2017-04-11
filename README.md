```
$ virtualenv --python=python3 venv && cd venv && source bin/activate
$ git clone git@github.com:imflop/superset.git
$ cd superset
```

```
# install for development
$ python setup.py develop
```

```
# Create an admin user
$ fabmanager create-admin --app superset
```

```
# Initialize the database
$ superset db upgrade
```

```
# Create default roles and permissions
$ superset init
```

```
# Load some data to play with
$ superset load_examples
```

```
# start a dev web server
superset runserver -d
```

```
# Into new terminal window, go to assets folder
$ cd superset/assets
```

```
# install depend.
$ npm install -i
```

```
# this part not work correct
# Copies a conf file from the frontend to the backend
$ npm run sync-backend
```

```
# Compiles the production / optimized js & css
$ npm run prod
```

```
# Start a web server that manages and updates your assets as you modify them
$ npm run dev
```

```
# For every development session you will have to
# start a flask dev server as well as an npm watcher

$ superset runserver -d -p 8081
$ npm run dev
```