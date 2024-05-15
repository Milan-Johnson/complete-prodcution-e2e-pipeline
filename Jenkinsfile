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
        stage('Checkout from SCM'){
            steps {
                git(url: 'https://github.com/Milan-Johnson/curriculum-app', branch: 'master')
            }
        }
        stage('Build Application'){
            steps {
                sh "mvn clean package"
            }
        }
        stage('Test Application'){
            steps {
                sh "mvn test"
            }
        }
    }
}
