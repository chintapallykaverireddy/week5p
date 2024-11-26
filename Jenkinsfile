pipeline {
  agent any 
  stages {
    stage('Building') {
       steps {
         script {
           bat "docker build -t week5p ."
           bat "docker run -d -p 3006:3006 week5p"
         }
       }
    } 
    stage('Runnig'){
      steps{
        script {
          echo "running the file"
        }
      }
    }
    stage('Testing'){
      steps {
        script {
          echo "testing"
        }
      }
    }
  }
}
  
