pipeline {
  agent any
    stages {
     stage('git clone') {
       steps {
         echo 'clone the repo'
          }
        }
   stage('build') {
    steps {
      sh '''echo PATH = ${PATH}
mvn -N io.takari:maven:wrapper
chmod +x mvnw
./mvnw clean install'''
      }
    }
