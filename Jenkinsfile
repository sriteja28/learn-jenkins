pipeline {
    agent { node { label 'workstation' } }

    environment {
        SSH = credentials('SSH')
        DEMO_URL = "google.com"
    }

    stages {
        stage('Hello-1') {
            steps {
                echo 'Hello World'
                sh 'env'
            }
        }
    }

    post {
        always {
            sh 'echo Post'
        }
    }

}
