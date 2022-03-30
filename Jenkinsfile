pipeline {
    agent any

    stages {
        stage('CloneRepo') {
            steps {
                dir ('code') {
                    checkout([
                    $class: 'GitSCM', branches: [[name: '*/branchname']], 
                    userRemoteConfigs: [[url: 'https://github.com/mendix/docs.git']]
                    ])
                }
            }
        }
    }
}