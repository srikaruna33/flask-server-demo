pipeline { 
    agent any 
    stages {
        stage('clean'){
            steps{
                cleanWs()
            }
        }
        stage('clone') { 
            steps {  
                git 'https://github.com/srikaruna33/flask-server-demo.git'
            }
        }
        stage('Deploy') {
            steps {
                sh 'docker-compose up'
            }
        }
    }
}
