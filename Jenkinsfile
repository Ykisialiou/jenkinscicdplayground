pipeline {
    agent { label "worker1" }

    stages {
        stage('CloneRepo') {
            steps {
                dir ('code') {
                    checkout([
                    $class: 'GitSCM', branches: [[name: 'master']], 
                    userRemoteConfigs: [[url: 'https://github.com/minamijoyo/myaws.git']]
                    ])
                }
            }
        }
    }
}