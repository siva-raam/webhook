
pipeline {
   agent { node { label 'test' } }

    stages {
        stage('Deploying docker on docker host-----------------') {
            steps {
		docker -H tcp://3.36.90.106 rm -f nginx-web1
                docker -H tcp://3.36.90.106 run -dit --name nginx-web1 -p 8000:80 nginx
            }
        }
    }
}
