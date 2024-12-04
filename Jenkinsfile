pipeline {
    agent any
    stages {
        stage('SonarTest') {
            steps {
                sh '''#!/bin/bash
                pwd
                sonar-scanner -Dsonar.host.url=http://192.168.4.7:9000 -Dsonar.token=sqp_3349de83b434e27196a88b9e646d37594bc72323
            '''
            }
        }
    }
}
