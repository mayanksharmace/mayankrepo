pipeline {
	agent any
	stages {
		stage('One') {
			steps {
				echo 'Hi, this is Soumitra from roytuts'
			}
		}

		stage('Two') {
			steps {
				input('Do you want to proceed?')
			}
		}

		stage('Build') {
            steps {
             - chmod +x './gradlew build'
            }
        }

        stage('Test') {
            steps {
            - chmod +x './gradlew test'
            }
        }

        stage('Check') {
            steps {
            - chmod +x './gradlew check'
            }
        }

		stage('Five') {
			steps {
				echo 'Finished'
			}
		}
	}
}
