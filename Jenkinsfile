pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                sh "sudo npm install"
                sh "sudo npm run build"
            }
        }
        stage("Deploy") {
            steps {
                sh "sudo rm -rf C:/jenkins-react-app"
                sh "sudo cp -r ${WORKSPACE}/build/ C:/jenkins-react-app/"
            }
        }
    }
}

