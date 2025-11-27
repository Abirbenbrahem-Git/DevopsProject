pipeline {
    agent any

    stages {
       stage('Checkout') {
            steps {
                checkout scmGit(
                    branches: [[name: '*/main']],
                    extensions: [],
                    userRemoteConfigs: [[url: 'https://github.com/Abirbenbrahem-Git/DevopsProject.git']]
                )
            }
        }

        stage('Compile') {
            steps {
                sh 'mvn clean compile'
            }
        }


    }
}
