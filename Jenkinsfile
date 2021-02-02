pipeline {
    
   agent any
   
  stages {
      
     stage('Run gcloud version') {
        steps {
           sh 'gcloud --version'
        }
     }
      
     stage('compute VM create') {
        steps {
           sh 'gcloud compute instances delete gcloud --zone=us-central1-a'
        }
     }
     
     stage('list vm instances') {
        steps {
           sh 'gcloud compute instances list'
        }
     }
  }
}
