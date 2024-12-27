pipeline {
    agent any  // This means the pipeline will run on any available Jenkins agent

    stages {
        // Stage to clone the repository
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/MinaHany98/20216105.git', branch: 'main'
            }
        }
        
        // Stage to execute the bash script
        stage('Execute Bash Script') {
            steps {
                sh './list_files.sh'  // This will run the script in the repository
            }
        }
    }
}
