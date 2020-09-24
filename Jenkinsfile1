@Library('shared-library@master') _
pipeline {
    agent any

    stages {
        stage('Git Checkout') {
            steps{
               
                gitCheckout(
                    branch: "master",
                    url: "https://github.com/musthu1837/multi-branch-pipe-line.git"
                )
            }
        }    
        stage("Build"){
            steps{
                script{
                    buildSystems.mavenBuild()
                }
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
