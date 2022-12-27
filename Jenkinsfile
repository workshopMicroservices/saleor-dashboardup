Pipeline {
    agent any
    stages {
        stage('VPC') {
            steps {
                git branch: 'main', url: 'https://github.com/workshopMicroservices/saleor-dashboardnew.git'
            }
        }
        stage('Build docker image') {
            steps {
                sh ('docker image build -t practice/saleor-dashboard:DEV .')
            }
        }
    }
}