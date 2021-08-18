pipeline {
  agent any
  stages {
    stage('check out code') {
      steps {
        git(url: 'https://github.com/EranFass/spring-boot-examples.git', branch: 'eran_sol', changelog: true)
      }
    }

  }
}