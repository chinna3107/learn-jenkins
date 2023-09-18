pipeline {
  //  agent any
    agent { node {label 'workstation1'} }

    environment {
       Test_URL = " google.com"
   }

    stages {
        stage('Compile') {
            steps {
                //echo 'Hello World'
                //error ' This is an error '
                echo Test_URL
            }
        }
    }
post {
 always{
  echo 'post'
   //send mail
   // Trigger some other job
   // Update some JIRA status about this build.
    }
  }
}
