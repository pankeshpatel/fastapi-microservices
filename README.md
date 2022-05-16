<p align="center">
  <img src="img/arch.png" width="500" title="app architecture">
</p>

```
// To create a virtual environment on mac

python3 -m venv venv
// step to enable vitual environmant in vs code
view -> command palette -> python:select interpreter -> ./venv/bin/python

we also need to enable virtual environment in terminal
source venv/bin/activate
```

```
//list all packages installed in virtual environment
pip freeze
// to install all packages
pip install -r requirements.txt

// to uninstall
pip uninstall $(pip freeze) -y
```

#### redis on mac

```
// installation link - https://redis.io/docs/getting-started/installation/install-redis-on-mac-os/
brew update // redis installation
brew install redis // redis installation
brew uninstall redis // redis uninstllation
brew services start redis  // to start redis service
redis-cli ping  // to check redis is running
brew services stop redis  // to stop service
```

```
redis document - https://redis.io/docs/getting-started/

redis-cli // commandline interface to interact with redis
keys * // list all the keys inside the redis (key-value store)
set usename pankeshpatel  // this would set a key-value in redis
get usename // to reterieve value of key "username"
get password // to ret value of key "password"
del <key-name> // to delete key
```
