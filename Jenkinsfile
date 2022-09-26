#Scripted pipeline script

node{
    stage ('spc-git'){
        git url: 'https://github.com/ganeshpatro98/spring-petclinic.git',
            branch: 'main'
    }
    stage('build'){
        bat 'mvn package'
    }
}

---
#Declarative pipeline script

pipeline{
    agent any
    stages{
        stage ('demo'){
            steps{
                echo 'hello world'
            }
        }
        stage ('spc-git'){
            steps{
                git url: 'https://github.com/ganeshpatro98/spring-petclinic.git',
                branch: 'main'
            }
        }
        stage ('build'){
            steps{
                bat 'mvn package'
            }
        }
    }
}