pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'Message1'
        writeFile(file: 'NewFileFromJenkins.txt', text: 'This is from the Jenkins Pipeline')
      }
    }
    stage('Stage2') {
      steps {
        fileExists 'NewFileTest.txt'
      }
    }
  }
}