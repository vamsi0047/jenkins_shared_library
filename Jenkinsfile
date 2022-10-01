@Library('vamsi@main') _
pipeline{
    agent none
    stages{
        stage("build"){
            steps{
                script{
                    build()
                }
            }
        }
         stage("sonar"){
            steps{
                script{
                    sonar.sonar()
                }
            }
        }
                 stage("sonar"){
            steps{
                script{
                    nexus.nexus()
                }
            }
        }
    }
}
