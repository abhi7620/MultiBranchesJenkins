pipeline {
    agent any
    parameters
	  {
		choice(name: 'VERSION', choices: ['1.1.0','1.1.1','1.1.2'], description: '')
        booleanParam(name: 'executeTest', defaultValue: true, description: '') 		
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
              echo "Build Test ${env.JOB_NAME}"  
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Build Deploy' 
				echo "Deploying version ${params.VERSION}" 
            }
        }
    }
}
