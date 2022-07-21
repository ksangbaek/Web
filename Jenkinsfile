pipeline {
    agent any
	
	//options { 
	//	disableConcurrentBuilds()
	//}
	
	parameters {
        choice( name: 'phase', choices: ['DEV', 'UAT', 'QA'] , description: "Choose Phase?" )
    }
	
    stages {
		stage('Init') {
            steps {
                echo "${env.BRANCH_NAME}"
            }
        }
		
        stage('Build') {
            steps {
                echo 'Building..'
			//	sleep time: 2, unit: 'MINUTES'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}