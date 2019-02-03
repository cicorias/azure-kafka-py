# Using Azure Event Hub's Kafka API Endpoint with Python 

This example is take from - https://github.com/Azure/azure-event-hubs-for-kafka/tree/master/quickstart/python

The following is still outstanding

- [ ] Update Consumer example
- [ ] Document additional installs and library dependancies
    - [ ] macOS
    - [ ] Windows
    - [ ] Debian

# Clone this repo

```
git clone git@github.com:cicorias/azure-kafka-py.git
cd ./azure-kafka-py

```

## CA Certificates
This repo contains the CA certs generated and used in Mozilla. The file `cacert.pem` comes from https://curl.haxx.se/docs/caextract.html


## Environment Variables
You must set the following either directly or create a `.env` file located in the same location -- `./src/.env`

```
BOOTSTRAP_SERVERS=<ourNameSpace>.servicebus.windows.net:9093
SERVICE_BUS_CONNECTION_STRING==<Get from Azure Keys>
```

## Developer Setup
The following are steps for installing pyenv on different operating systems. The first is macOS

- [ ] Add debian
- [ ] Add windows

### maxOS Install Pyenv

```
curl https://pyenv.run | bash
# then add the commands shown to .bashrc or .bash_profile
vi /Users/cicorias/.bash_profile
exec -l $SHELL
```

#### Install Python 3.7.2 under Pyenv

First ensure a few dependencies are in place.

```
brew update
brew install openssl
brew install readline xz
```

- On macOS 10.14 or higher, you must add some SDK headers / libraries to an old location as pyenv hasn't been updated to look in the new default paths.

```
sudo installer -pkg /Library/Developer/CommandLineTools/Packages/macOS_SDK_headers_for_macOS_10.14.pkg -target /
```


- Run the Pyenv install
```
pyenv install  3.7.2
```

- Set the current shell's Python to 3.7.2 -- and then create a virtual env

```
pyenv shell 3.7.2
python -m venv env
. ./env/bin/activate
```

>At this point you should have an isolated Python install running Python 3.7.2.

# Installing Requirements
From the root of the cloned repo directory run:
```
pip install -r requirements.txt

```




