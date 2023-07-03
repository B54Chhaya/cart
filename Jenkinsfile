pipeline{
    agent{
        label "ws"
    }
    stages{
        stage("lint checks"){
            steps{
                sh  "cd cart/home/centos/node_modules/jslint/bin/jslint.js server.js"
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
    
}