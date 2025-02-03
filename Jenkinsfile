pipeline {
    agent any

    stages {
        stage('Test necesary tools') {
            steps {
                sh '''
                    npm --version
                    git --version
                '''
            }
        }

        stage("Build"){
            steps{
                sh '''
                    ls -a 
                '''
            }
        }
    }
}