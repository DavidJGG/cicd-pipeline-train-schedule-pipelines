pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Construyendo por segunda vez .....'
                sh './gradlew build --no-daemon' 
                archiveArtifacts artifacts: 'dist/trainSchedule.zip', fingerprint: true 
            }
        }
    }
}
