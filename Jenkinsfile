pipeline {
  
  agent any
  
  stages{
    stage ('B. Maven Build'){ 
      steps{
        sh 'mvn clean package'
      }
    }
  }
     post{
       success{
         emailext body: 'Email sent out from Jenkins', subject: 'Test Email', to: 'devopsstudygroup@gmail.com'
       }
     }
}
