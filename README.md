## Build an Image ##

```docker build --tag x01188 .```

## Run an image ##

```docker run --name x01188C -p 8090:8080 x01188```

## If you are using windows operating system try to run the below command before running the CURL commands ##

```Remove-item alias:curl```

## Run the curl command ##

This transfers ETH:

```curl -i -X POST -H "Content-Type: application/json" -d '{\"address\": \"0xb41243470b3f379fbFe652d69c742207336A7A5e\",\"amount\":\"0.05\"}' http://localhost:8090/eth```
                                                                            
This transfers token:

```curl -i -X POST -H "Content-Type: application/json" -d '{\"address\": \"0xb41243470b3f379fbFe652d69c742207336A7A5e\"}' http://localhost:8090/token```