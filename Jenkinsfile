pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "compilation"
                sh 'make.sh' 
                archiveArtifacts artifacts: 'code', fingerprint: true 
            }
        }
    }
}
