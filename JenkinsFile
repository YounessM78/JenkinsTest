pipeline {
    agent any
    
    stages {
    
        stage('Checkout') {
            steps {
               checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], gitTool: '', userRemoteConfigs: [[url: 'https://github.com/YounessM78/JenkinsTest.git']]])
            }
        }
        stage('Build') {
            steps {
                git branch: 'main', url: 'https://github.com/YounessM78/JenkinsTest.git'
                bat label : '', script :'C:\\Users\\a864467\\AppData\\Local\\Programs\\Python\\Python310\\python.exe test.py'
                
            }
        }
        stage ('test') {
            steps {
            echo 'le boulot a été fait'
            }
        }
        
       
    }
}
