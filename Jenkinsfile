pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh 'git clone https://github.com/VulcanClimateModeling/fv3gfs-fortran.git'
            }
        }
    }
    post {
        success {
            sh 'rm -rf fv3gfs-fortran'
        }
    }
}
