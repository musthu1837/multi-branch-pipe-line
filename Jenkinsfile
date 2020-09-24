pipeline {
    agent any

    stages {
        stage("Build"){
            steps{
                sh "mvn clean package"
            }
        }
        stage("Dev") {
            steps {
                echo "Started stage Dev"
            }
        }

        stage("Prod") {
            steps {
                echo "Started stage prod"
            }
        }
    }
}
