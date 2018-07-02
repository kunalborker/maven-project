pipeline {
  agent any
    stages{
      stage ('Compile stage'){
        steps{
          maven(maven : 'localMaven'){
          sh 'mvn clean compile'
          }
        }
      }
      stage ('Testing stage'){
        steps{
          maven(maven : 'localMaven'){
          sh 'mvn test'
          }
        }
      }
      stage ('Deploy stage'){
        steps{
          maven(maven : 'localMaven'){
          sh 'mvn deploy'
          }
        }
      }
    }
}
