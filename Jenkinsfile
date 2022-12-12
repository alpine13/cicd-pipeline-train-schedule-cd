pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'DeployToStaging'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
