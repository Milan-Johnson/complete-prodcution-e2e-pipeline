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
                git(url: 'https://github.com/Milan-Johnson/curriculum-app', branch: 'master')
            }
        }
    }

}
