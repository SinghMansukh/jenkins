pipeline{
    agent any 
    stages{
        stage("Test"){
            steps{
                echo "========executing the BUILD_NUMBER. the ID is $BUILD_NUMBER========"
                
            }
            post{
                always{
                    echo "========always========"
                }
                success{
                    echo "========A executed successfully======="
                }
                failure{
                    echo "========A execution failed========"
                }
            }
        }
        stage("Dev"){
            steps{
                echo "========executing BUILD URL i.e $BUILD_URL========"
                echo "========executing JENKINS URL i.e $JENKINS_URL========"
                echo "========executing NODE NAME i.e $NODE_NAME========"
                echo "========executing WORKSPACEL i.e $WORKSPACE========"
                
            }
            post{
                always{
                    echo "========always========"
                }
                success{
                    echo "========A executed successfully========"
                }
                failure{
                    echo "========A execution failed========"
                }
            }
        }
        stage("ENV "){
            steps{
                echo "========executing Prod========"
            }
            post{
                always{
                    echo "========always========"
                }
                success{
                    echo "========A executed successfully========"
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
