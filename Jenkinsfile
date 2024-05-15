pipeline{
    agent any

    tools{
        jdk 'Java17'
        maven 'Maven3'
    }
    stages {
        stage("Cleanup Workspace"){
            steps {
                cleanWs()
            }
        }
    }

    stages {
        stage('Checkout from SCM'){
            steps {
                git branch: 'main', url: 'https://github.com/Milan-Johnson/complete-prodcution-e2e-pipeline'
            }
        }
    }

}
