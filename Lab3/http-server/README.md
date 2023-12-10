docker build server .

docker run -p 8080:8080 server

wrk -t10 -c500 -d60s http://0.0.0.0:8080/
