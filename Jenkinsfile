pipeline {
  agent any
  stages {
    stage('check out code') {
      steps {
        git(url: 'https://github.com/EranFass/spring-boot-examples.git', branch: 'eran_sol', changelog: true)
      }
    }

    stage('maven compile') {
      steps {
        sh '''cd spring-boot-package-war
mvn compile'''
      }
    }

    stage('test') {
      steps {
        sh '''cd spring-boot-package-war
mvn test'''
        sh '''cd spring-boot-package-war
mvn test'''
      }
    }

  }
}