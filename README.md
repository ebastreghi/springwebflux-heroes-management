Spwing Webflux, AWS SDK, Swagger, DynamoDB, JUnit

Enable AWS Access Key
Install AWS CLI
Open terminal and type: aws configure

Download local DynamoDB in tyhe link bellow
https://docs.aws.amazon.com/pt_br/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html

Execute the command bellow in the directory that you extract the zip file
java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb


Acces DynamoDB in localhost
aws dynamodb list-tables --endpoint-url http://localhost:8000