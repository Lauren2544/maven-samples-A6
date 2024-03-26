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
        sh '''git bisect start 198644632661c67b6c32f59e9047c11a70685e15 98ac319c0cff47b4d39a1a7b61b4e195cfa231e5
git bisect run mvn clean test
'''
      }
    }

  }
  tools {
    maven 'MVN 1'
    jdk 'JDK version 1.8.0_221'
  }
}