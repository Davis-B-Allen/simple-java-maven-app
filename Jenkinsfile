pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            args ' -v /tmp/.m2:/tmp/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo HERE'
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}
