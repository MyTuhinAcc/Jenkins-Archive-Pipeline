pipeline {
    agent any

    stages {

        stage('Generate Report') {
            steps {
                bat '"C:\\Users\\TUHIN BHATTACHARYA\\AppData\\Local\\Programs\\Python\\Python312\\python.exe" app.py'
            }
        }

        stage('Archive Report') {
            steps {
                archiveArtifacts artifacts: 'report.txt',
                    fingerprint: true
            }
        }
    }
}