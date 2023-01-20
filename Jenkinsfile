pipeline {
   agent any
   tools {
      gradle 'Gradle'
      }
      stages {
         stage ("run frontend") {
            steps {
               echo 'executing yarn'
               nodejs('NodeJS-10') {
                 sh 'yarn installl'
                 }
               }
             }
          stage ("run backend") {
             steps {
                 echo 'executing gradle'
                 sh './gradlew -v'
                 }
               }
             }
      }
