pipeline{
    agent none

    stages{
        stage('Test'){
            step{
                sh 'docker container run -v "$(pwd)":/usr/src/mymaven -w /usr/src/mymaven maven:3-openjdk-8 mvn clean package'
            }
        }
    }
}