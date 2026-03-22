pipeline {
  agent any
  tools {
      maven '3.9.6'
      jdk 'JDK 8'
  }
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/Riceria/maven-samples-A6', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn clean test'
      }
    }

  }
}
