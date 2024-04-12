pipeline{
    agent any
    tools{
        gradle 'gradle'
    }
    stages{
        stage('clone code'){
           steps{
               git branch: 'master', url: 'https://github.com/IvyMachogu/java-todo.git'
           }
    }
    stage('gradle code'){
        steps{
            sh 'gradle build'
        }
        
       }
       stage('test code'){
           steps{
               sh 'gradle test'
           }
       }
    }
}