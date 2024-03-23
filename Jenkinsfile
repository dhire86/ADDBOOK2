pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "testmaven"
    }
//untracked 

parameters{
    string(name:'Env',defaultValue:'Dev',description:'this is for env app')
    booleanParam(name:'execution',defaultValue:'true',description:'check the execution')
    choice(name:'appversion',choices:['1.1','1.2','1.3'])
}
    stages {
        stage('compilecode4') {
            steps {
    choice(name:'appversion',choices:['1.1','1.2','1.3'])
                echo " this is code compile for pipeline 4 ${params.appversion}"
            }
        }
    
    stage('Testunit4') {
            steps {
                echo " this is code unit test for pipeline 4 "
            }
    }
    stage('Package4') {
            steps {
                echo " this is code  package for pipeline 4 ${params.Env}"
           ls statu }
        }
    }
}
