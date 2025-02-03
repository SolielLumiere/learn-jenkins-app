pipeline {
    agent any

    stages {
        cleanWs()
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
                    node --version
                    npm --version
                    npm install
                    npm run build
                '''
            }
        }
    }
}