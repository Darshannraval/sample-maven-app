pipeline {
    agent any
    tools {
        maven "Maven"
    }
    
     triggers {
        pollSCM "* * * * *"
    }
    stages{
        stage("Build"){
            steps{
                 sh script: 'mvn clean package'
            }
        }
}

}
