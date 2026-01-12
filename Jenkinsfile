pipeline {
    agent any

    stages {

        stage('PULL') {
            steps {
                git 'https://github.com/adityakashid/batch21.git'
            }
        }

        stage('BUILD') {
            steps {
                dir('backend') {
                    sh 'mvn clean package -DskipTests'
                }
            }
        }

	}
}
