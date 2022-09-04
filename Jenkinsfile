pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
               echo 'Build Application'
            }
        }
        stage('Test') {
			when{
				expression{
					BRANCH_NAME == 'main'
				}
			}
            steps {
              echo 'Build Test'  
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Build Deploy' 
            }
        }
    }
}
