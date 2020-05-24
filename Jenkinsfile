pipeline {
    agent any
    tools {
        maven 'maven 3.3.9'
    }
    stages{
        stage('Build'){
            steps{
                 sh script: 'mvn clean package'
                 archiveArtifacts artifacts: 'target/*.war', onlyIfSuccessful: true
            }
        }
}

}
