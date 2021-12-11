
pipeline {
   agent { node { label 'test' } }

    stages {
        stage('Deploying docker on docker host-----------------') {
            steps {
		sh 'docker -H tcp://3.36.90.106 rm -f nginx-web2'
                sh 'docker -H tcp://3.36.90.106 run -dit --name nginx-web2 -p 8800:80 nginx'
            }
        }
    }
}
