pipeline {
    agent any
    environment{
      NEW_VERISION = '1.3.0'
      JOB_NAME = JOB_NAME
    }
    stages {
        stage('Build') { 
            steps {
               echo 'Buliding the application'
               echo 'Build Application $(NEW_VERISION)'
            }
        }
        stage('Test') {
			      steps {
              echo 'Build application Test'
              echo 'Build Test $(JOB_NAME)'  
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Build Deploy' 
            }
        }
    }
}
