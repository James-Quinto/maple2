ppipeline {
    agent {
    }
    stages {
        stage('Build Node JS Container') {
            steps {
                //sh 'npm install'
            }
        }
        stage('Test application / Smart Check Scans') {
            steps {
                //sh './jenkins/scripts/test.sh'
            }
        }
        stage('Deliver for development') {
            when {
                branch 'development' 
            }
            steps {
                //sh './jenkins/scripts/deliver-for-development.sh'
                //input message: 'Finished using the web site? (Click "Proceed" to continue)'
                //sh './jenkins/scripts/kill.sh'
            }
        }
        stage('Deploy for production') {
            when {
                branch 'production'  
            }
            steps {
                //sh './jenkins/scripts/deploy-for-production.sh'
                //input message: 'Finished using the web site? (Click "Proceed" to continue)'
                //sh './jenkins/scripts/kill.sh'
            }
        }
    }
}
