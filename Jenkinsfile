pipeline {
	agent any
	stages {
		stage('One') {
			steps {
				echo 'This is step One'
			}
		}

		stage('Two') {
			steps {
				input('Do you want to proceed?')
			}
		}

		stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                echo 'This is step Test'
            }
        }

        stage('Check') {
            steps {
                echo 'This is step Check'
            }
        }

		stage('Five') {
			steps {
				echo 'Finished'
			}
		}
	}
}