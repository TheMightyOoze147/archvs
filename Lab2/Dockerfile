FROM gcc:latest

COPY main.cpp /app/main.cpp

WORKDIR /app

RUN g++ -o /app/main /app/main.cpp

CMD ["/app/main"]
