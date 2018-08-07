# Circuit-Breaker
# Clean and build both apps
mvn clean install
# Run application
java -jar target\spring-hystrix-school-service-0.0.1-SNAPSHOT.jar. 
---- This will start the school service in default port 9098.
# Hit the URL to check if app is running
http://localhost:9098/getSchoolDetails/abcschool. It should show the below output in browser 

# Hystrix Dashboard
As we have added hystrix dashboard dependency, hystrix has provided one nice Dashboard and a Hystrix Stream in the bellow URLS:

http://localhost:9098/hystrix.stream – It’s a continuous stream that Hystrix generates. It is just a health check result along with all the service calls that are being monitored by Hystrix. Sample output will look like in browser

# This is visual dashboard initial state.
http://localhost:9098/hystrix – 

# Enter http://localhost:9098/hystrix.stream  in Dashboard to display metrics
