pipeline {
   agent any

   stages {
      stage('Build') {
         steps {
            echo 'Start building...'
         }
      }
      stage('NUnit') {
          steps {
            echo 'Start NUnit testing...'
          }
      }
      stage('Deploy') {
          steps {
             echo 'Start Deploy...' 
          }
      }
      stage('Integration') {
          steps {
            echo 'Start integration & testing...'
          }
      }
   }
   
   post {
       always {
           echo 'This will always run'
       }
       success {
           echo 'This will run if success'
       }
       failure {
           echo 'This will run if fails'
       }
       unstable {
           echo 'This will run if it is marked unstable'
       }
       changed {
           echo 'This will run if state changed'
       }
   }
}
