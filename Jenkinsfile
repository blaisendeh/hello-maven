pipeline {
     agent any
     options {
         timeout(time: 10, unit: 'MINUTES')
     }
     stages {
         stage('VALIDATE THE MAVEN PROJECT') {
             steps {
               sh 'mvn validate'
             }
         }
     }


