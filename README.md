# Microprofile Health Check & Metrics understanding

Sample REST operations.

## Build and run

myself all build folder generated using JDK14 if you do not have please delete build folder and generate your version target folder
```bash
mvn package
java -jar target/demo-health.jar
```

## Test local links for demo

```
http://localhost:8080/greet
{"message":"Hello My Microprofile World!"}

 GET http://localhost:8080/greet/Prabu
{"message":"Hello Prabu!"}

"Content-Type: application/json" -d '{"greeting" : "Hi"}' http://localhost:8080/greet/greeting

GET http://localhost:8080/greet/Prabu
{"message":"Hi Prabu!"}
```

## Try health and metrics

```
http://localhost:8080/health
http://localhost:8080/metrics
 ## Please use local any container environment to run  eg doucker 
