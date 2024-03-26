<<<<<<< HEAD
    pipeline {
=======
pipeline {
>>>>>>> d733a83e38ed7a85c61f4d3c4bcffe1e904b518b
    agent none

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "testmaven"
    }
parameters {
    choice(name:'appversion',choices:['1,1','1.2'])
   
}
    
//untracked 
    stages {
        stage('compilecode4') {
            agent {label 'slavejenkins'}
            steps {
                echo " this is code compile for pipeline 4 ${params.appversion}"
                sh 'mvn compile'
            }
        }
    
    stage('Testunit4') {
          agent any
            steps {
                echo " this is code unit test for pipeline 4"
                sh 'mvn test'
            }
    }
    stage('Package4') {
        agent any
            steps {
                echo " this is code  package for pipeline 4  "
                sh 'mvn package'
            }
        }
    }
}