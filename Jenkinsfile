pipeline {
   agent any
   stages {
       stage('Testing multi-branch pipeline') {
            when {
               branch 'Prod'
            }   
            steps {
               input message: 'Do you want to proceed?', submitter: 'Administrator'
               sh "echo 'This is from ${BRANCH_NAME}...'"
            }
       }
   }
}   
