# SpringBootDemoApp
SpringBootDemoApp

Launch https://start.spring.io/ to download basic SpringBoot application with all dependencies we want

GoThrough the REST Api guide in in https://projects.spring.io/spring-boot/#quick-start

cf login api http://api.run-np.<pcfProvider>.com

cf target -o <Org_Name> -s <Space_Name>

Go into your app folder to deploy our already built jar

cf push -p build/libs/demo-0.0.1-SNAPSHOT.jar -m 256M


Create User Provided services
cf cups sample.db2.service -p "{\"jdbcUrl\":\"jdbc:Db2://<URL>:<Port>/<Schema/db>:user=<UserName>;password=<Password>;\"}“
