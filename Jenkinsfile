Pipeline {
    agent any
    stages {
        stage('VPC') {
            steps {
                git branch: 'main', url: 'https://github.com/workshopMicroservices/saleor-dashboardup.git'
            }
        }
        stage('Build docker image') {
            steps {
                sh ('docker image build -t practice/saleor-dashboard:DEV .')
            }
        }
    }
}