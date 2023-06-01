node {
    stage ('clone') {
        git 'https://github.com/koteswararao73/DockerWebProject.git'
    }
    stage ('image build') {
        sh ''' docker build -t koti . '''
    }
    stage ('run container') {
        sh ''' docker run --name koti12 -d -p 85:80 koti '''
    }
}
