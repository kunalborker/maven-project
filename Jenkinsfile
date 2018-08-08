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
}
}
