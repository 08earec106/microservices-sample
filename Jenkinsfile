pipeline{
    agent {
        docker { image 'node:16.13.1-alpine' }
    }
    stages{
        stage('Test') {
            steps{
                sh 'docker container run -v "$(pwd)":/usr/src/mymaven -w /usr/src/mymaven maven:3-openjdk-8 mvn clean package'
            }
        }
    }
}