# Using Azure Event Hub's Kafka API Endpoint with Python 

This example is take from - https://github.com/Azure/azure-event-hubs-for-kafka/tree/master/quickstart/python

The following is still outstanding

- [ ] Update Consumer example
- [ ] Document additional installs and library dependancies
    - [ ] macOS
    - [ ] Windows
    - [ ] Debian



## CA Certificates
This repo contains the CA certs generated and used in Mozilla. The file `cacert.pem` comes from https://curl.haxx.se/docs/caextract.html


## Environment Variables
You must set the following either directly or create a `.env` file located in the same location -- `./src/.env`

```
BOOTSTRAP_SERVERS=<ourNameSpace>.servicebus.windows.net:9093
SERVICE_BUS_CONNECTION_STRING==<Get from Azure Keys>
```

