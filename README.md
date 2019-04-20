# tp-speedtest
Dette er Speedtest server igennem docker.

For at starte containeren kan du skrive:
````
docker run -itd --name speedtest -p 80:80 ilasiaq88/tp-speedtest
````

For at køre det med docker-composer kan du anvende:
````
version: '3'
services:
  speedtest:
    image: "ilasiaq88/tp-speedtest"
    container_name: speedtest
    ports:
      - 80:80
````

*This is taken from [adolfintel/speedtest](https://hub.docker.com/r/adolfintel/speedtest)*
