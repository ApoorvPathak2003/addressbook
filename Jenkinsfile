pipeline {
    agent any
    stages {
        stage('Build/Compile') {
            steps {
                sh 'mvn clean compile package'
            }
        }
    }
}

pipeline {
    agent any
    stages {
        stage('Build/Compile') {
            steps {
                sh 'mvn clean compile package'
            }
        }
        stage('Code-Review') {
            steps {
                sh 'mvn checkstyle:checkstyle'
            }
        }
    }
}

pipeline {
    agent any
    stages {
        stage('Build/Compile') {
            steps {
                sh 'mvn clean compile package'
            }
        }
        stage('Code-Review') {
            steps {
                sh 'mvn checkstyle:checkstyle'
            }
        }
        stage('Unit-Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
