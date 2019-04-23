pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Running Building..Automation'
                sh './gradlew build --no-daemon'
                archveArtifacts artifacts: 'dist/trainSchedule.zip'
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
