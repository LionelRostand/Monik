pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.46    mkdir /applis'
                 sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.46   export Home_applis=/applis'
                 sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.46   chown youtechadmin:youtechadmin /applis'
            }

        }
        stage('SUPPRESSION') {
            steps {
                sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.46   rmdir /applis'
               
            }

        }
       
    }
    
}

