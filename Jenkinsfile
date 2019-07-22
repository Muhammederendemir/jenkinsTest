
pipeline {
   agent any
   stages {
       stage('Compile') {
          steps {
               catchError {
                   sh './gradlew compileJava --stacktrace'
               }
           }
           post {
               success {
                   echo 'Compile stage successful'
               }
               failure {
                   echo 'Compile stage failed'
               }
           }
       }
       /* ... other stages ... */
   }
   post {
       success {
           echo 'whole pipeline successful'
       }
       failure {
           echo 'pipeline failed, at least one step failed'
       }
   }