pipeline {
    agent {
        docker {
            image 'maven:3.9.2'
            args '-v /root/.m2:/home/ggg/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}
