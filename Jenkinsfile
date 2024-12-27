pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/MinaHany98/20216105.git', branch: 'main'
            }
        }

        stage('Execute Bash Script') {
            steps {
                sh 'chmod +x list_files.sh'
                sh './list_files.sh'
            }
        }
    }
}
