pipeline {
    agent {
        docker {
            image 'maven:3.9.2'
            args '-v /home/ggg/.m2:/.m2'
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
