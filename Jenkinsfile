pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(branch: 'master', url: 'https://github.com/Lauren2544/maven-samples-A6.git')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

  }
  tools { 
      maven 'MVN 1'
    jdk 'JDK version 1.8.0_221'
  }
  }

