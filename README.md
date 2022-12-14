## Download Docker Desktop application in your machine ##

## Running a docker container ##

## Method 1 ##
## Build an Image using the Dockerfile##

```docker build --tag image_name .```

## Run an image ##

```docker run --name container_name -p 8090:8080 image_name```

## Method 2 ##
## Using Docker compose file ##

```docker-compose up```

## Once Docker is up, run the following CURL commands ##

## Note : If you are using windows operating system try to run the below command before running the CURL commands ##

```Remove-item alias:curl```

## Run the curl command ##

## The below command transfer the mentioned Ether amount from the ower adderss to the given address ##
For Windows machine:

```curl -i -X POST -H "Content-Type: application/json" -d '{\"address\": \"Target Address\",\"amount\":\"Ether amount to be transfered\"}' http://localhost:8090/eth```

For Mac machine:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"Target Address", "amount":"Ether amount to be transfered"}' http://localhost:8090/eth```

## The below command transfer the mentioned Ether amount from the ower adderss to the given address ##
                                                                            
For Windows machine:

```curl -i -X POST -H "Content-Type: application/json" -d '{\"address\": \"Target Address\"}' http://localhost:8090/token```

For Mac machine:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"Target Address"}' http://localhost:8090/token```
