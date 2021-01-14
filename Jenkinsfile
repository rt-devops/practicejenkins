pipeline{
    agent{
        label "dockeragent"
    }
    stages{
        stage("build"){
            steps{
                echo "Project is building"
            }
            post{
                always{
                    echo "========always========"
                }
                success{
                    echo "========A executed successfully===="
                }
                failure{
                    echo "========A execution failed========"
                }
            }
        }
    }
    post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}