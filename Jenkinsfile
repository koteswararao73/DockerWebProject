pipeline { 
    agent any
    stages {
        stage ('clone') {
            steps {
                git 'https://github.com/koteswararao73/DockerWebProject.git'
                stage ('build image') {
                    steps {
                        sh 'docker build -t gabber . '
                stage ('run container') {
                    steps {
                        sh 'docker run --name scriprt -d -p 98:80 gabber '
                    }
                }
                    }
                }
            }
        }
    }
}
