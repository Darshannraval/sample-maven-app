pipeline {
    agent any
    tools {
        maven "M3"
    }
    
     triggers {
        pollSCM "* * * * *"
    }
    stages{
        stage("Build"){
            steps{
                 sh 'mvn -B -DskipTests clean package'
            }
        }
}

}
