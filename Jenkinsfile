pipeline {
    agent any
    stages {
        stage('SonarTest') {
            steps {
                sh "docker run --rm -e SONAR_HOST_URL="http://192.168.4.7:9000/" -e SONAR_TOKEN="sqp_3349de83b434e27196a88b9e646d37594bc72323" -v "$(pwd):/usr/src" sonarsource/sonar-scanner-cli"
            }
        }
    }
}
