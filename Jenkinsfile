node {
    stage ('clone') {
        git 'https://github.com/koteswararao73/DockerWebProject.git'
    }
    stage ('image build') {
        sh ''' docker build -t koti . '''
    }
    stage ('run container') {
        sh ''' docker run --name koti3211 -d -p 86:80 koti '''
    }
}
