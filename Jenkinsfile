pipeline {
  agent any
    tools { 
        maven 'Maven 3.3.9' 
    }
    stages{
      stage ('Compile stage'){
        steps{
          sh 'mvn clean compile'
        }
      }
      stage ('Testing stage'){
        steps{
          sh 'mvn test'
          }
      }
      stage ('Deploy stage'){
        steps{
          sh 'mvn deploy'
          }
      }
    }
}
