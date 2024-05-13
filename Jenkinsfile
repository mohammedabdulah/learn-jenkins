pipeline {
    agent {
        node {
            label 'AGENT-1'
        }
    }
    environment {
        GREETING = 'Hello Jenkins'
    }
    // options {
    //     timeout (time :1 , units: 'HOURS')
    // }
    // options {
    //     ansicolor ('xterm')
    // }
    
    parameters {
        string (name: 'PERSON' , defaultValue : 'Mr.Jenkins' , description: 'who are you')
        text (name: 'BIOGRAPHY' , defaultValue: '' , description: 'write something')
    }

        stages {
            stage ('Build') {
                steps {
                    sh """
                    echo "this is my first shell script in jenkins"
                    env
                    """
                    echo 'BUILDING'

                }
            }
            stage ('Test') {
                steps {
                    echo 'Testing'
                }
            }
            stage ('Deploy') {
                steps {
                    echo 'ENJOYING'
                }
            }
            stage ('EXAMPLE') {
                steps{
                    
                    echo "hello "
            
                
                }
            }
        }
    }