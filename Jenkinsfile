pipeline {
    agent any

    stages {
        stage('Build') {
            when {
                expression {
                env.BRANCH_NAME == 'development'
                }
            }
            steps {
                echo 'Gradlew version..'
                sh './gradlew --version'

                echo 'Building..'
                sh './gradlew build --no-daemon'
            }
        }
    }
    post {
        always {
            echo 'Post stage..'
        }
    }

    
}