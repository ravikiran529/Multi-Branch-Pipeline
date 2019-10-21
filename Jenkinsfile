pipeline {
   agent any
   stages {
       stage('Testing multi-branch pipeline') {
            steps {
               echo "This is from ${BRANCH_NAME}..."
               ech "Running on ${NODE_NAME}."
            }
       }
      post {
         failure {
            mail bcc: '', body: 'A Build has failed.Please have a look.', cc: '', from: '', replyTo: '', subject: 'Build failed!', to: 'rrkiran.529@gmail.com'
         }
     }
  }
}   
   
