pipeline {
    agent any
    stages {
        stage('Repo Clone') {
            steps {
                timeout(time: 3, unit: 'MINUTES') {
                    retry(3) {
                        sh 'git clone https://github.com/VulcanClimateModeling/fv3gfs-fortran.git'
                    }
                }
            }
        }
    }
    post {
        success {
            sh 'rm -rf fv3gfs-fortran'
        }
    {
}
