pipeline {
    agent any
    stages {
        stage('SonarTest') {
            steps {
                sh '''#!/bin/bash
                pwd
                ls
                curl -O -k https://binaries.sonarsource.com/Distribution/sonar-scanner-cli/sonar-scanner-cli-6.2.1.4610-linux-x64.zip
                unzip sonar-scanner-cli-6.2.1.4610-linux-x64.zip &&  mv sonar-scanner-6.2.1.4610-linux-x64 sonar-scanner
                ./sonar-scanner/bin/sonar-scanner -Dsonar.host.url=http://192.168.4.7:9000 -Dsonar.token=sqp_3349de83b434e27196a88b9e646d37594bc72323
            '''
            }
        }
    }
}
