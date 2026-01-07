pipeline {
                agent any 
                stages {
                    stage('Code Analysis') { 
                        steps {
                            sh 'uname' 
                        }
                    }
                    stage('Build') { 
                        steps {
                             sh 'cat /etc/os-release'
                        }
                    }
                    stage('Deploy') { 
                        steps {
                            sh 'sudo docker image ls'
                        }
                    }
                }
            }