pipeline {
    agent any

    tools {
        maven "maven"
    }
    stages {
        stage('git checkout') {
            steps {
               git 'https://github.com/rohithreddy-41/DevOPs.git'
		}
	}
	 stage('compile') {
            steps {
               bat "mvn compile"
		}
	}
	stage('test') {
            steps {
               bat "mvn test"
		}
	}
	stage('package') {
            steps {
               bat "mvn package"
		}
	}
	stage('build') {
            steps {
               bat "mvn install"
		}
	}
    }
}