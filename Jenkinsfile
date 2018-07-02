pipeline {
  agent any
    tools { 
        maven 'localMaven' 
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
