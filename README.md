Spring Webflux, AWS SDK, Swagger, DynamoDB, JUnit



Enable AWS Access Key
Install AWS CLI
Open terminal and type: aws configure

******************************************
Download local DynamoDB in tyhe link bellow
https://docs.aws.amazon.com/pt_br/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html
Execute the command bellow in the directory that you extract the zip file
java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb

OR

docker run -p 8000:8000 amazon/dynamodb-local -jar DynamoDBLocal.jar -inMemory -sharedDb
*******************************************

********************
Open the project
run the class com.springwebfluxheroesmanagement.config.HeroesTable to create the table
run the class com.springwebfluxheroesmanagement.config.HeroesData to populate the table
and then openthe url bellow to make tests with swagger 
http://localhost:8080/swagger-ui-heroes-reactive-api.html
********************

Acces DynamoDB in localhost
aws dynamodb list-tables --endpoint-url http://localhost:8000