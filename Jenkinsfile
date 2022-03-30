pipeline {
    agent any

    stages {
        stage('CloneRepo') {
            steps {
                dir ('code') {
                    checkout([
                    $class: 'GitSCM', branches: [[name: '*/development']], 
                    userRemoteConfigs: [[url: 'https://github.com/mendix/docs.git']]
                    ])
                }
            }
        }
    }
}
