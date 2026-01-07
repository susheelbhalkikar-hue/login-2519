pipeline {
                agent any 
                stages {
                    stage('Code Analysis') { 
                        steps {
                            echo 'Code Analysis'
                            sh 'sudo docker run  --rm -e SONAR_HOST_URL="http://3.14.255.46:9000" -v ".:/usr/src" sonarsource/sonar-scanner-cli -Dsonar.token=sqp_ab0da1dc85161f6037f912e07f0882e0b4377e2c -Dsonar.projectKey=lms' 
                        }
                    }
                    stage('Build') { 
                        steps {
                             sh 'cat /etc/os-release'
                        }
                    }
                    stage('Deploy frontline') { 
                        steps {
                            sh 'sudo docker image ls'
                        }
                    }
                }
            }