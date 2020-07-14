pipeline
{
agent any
stages{
   stage('Build Application'){
   steps{
   bat 'mvn clean install'
   }
   }

   stage('Deploy Application To Mulesoft Cloudhub'){
   steps{
   bat 'mvn package deploye -DmuleDeploy'
   }
   }

   stage('Perform Regression Testing'){
   steps{
   bat 'C:\\Users\\elias.moges\\AppData\\Roaming\\npm\\newman run C:\\Users\\elias.moges\\Documents\\newman\\Worldtimezone.postman_collection.json --disable-unicode'
   }
   }
   }
}
