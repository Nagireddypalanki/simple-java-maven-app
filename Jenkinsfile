pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                git url: 'https://github.com/Nagireddypalanki/simple-java-maven-app.git'
                withMaven {
                    sh 'mvn -B -DskipTests clean package' 
                }
            }
        }
    }
}
