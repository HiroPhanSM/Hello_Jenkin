pipeline{
    agent{
        label "node"
    }

    environment {
        TEST_ENVI = "-----hello jenkins-----"
    }

    stages{
        stage("Build"){
            steps{
                echo "========executing Build!========"
            }
            post{
                success{
                    echo "========Build executed successfully!========"
                }
                failure{
                    echo "========Build execution failed!========"
                }
            }
        }

        stage("Test"){
            steps{
                echo "========executing Test========"
            }
            post{
                success{
                    echo "========Test executed successfully========"
                }
                failure{
                    echo "========Test execution failed========"
                }
            }
        }

        stage("Deployment"){
            steps{
                echo "========executing Deployment========"
            }
            post{
                success{
                    echo "========Deployment executed successfully========"
                }
                failure{
                    echo "========Deployment execution failed========"
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