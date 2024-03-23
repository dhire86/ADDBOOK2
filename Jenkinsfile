pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "testmaven"
    }
//untracked 
    stages {
        stage('compilecode4') {
            steps {
                echo " this is code compile for pipeline 4"
            }
        }
    
    stage('Testunit4') {
            steps {
                echo " this is code unit test for pipeline 4"
            }
    }
    stage('Package4') {
            steps {
                echo " this is code  package for pipeline 4"
            }
        }
    }
}
