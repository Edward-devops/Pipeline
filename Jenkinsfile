pipeline {
   agent any
    stages {
        stage('GIt checkout') 
        {
            steps {
                echo "checking out"
                git credentialsId: '9dbd834d-9dc9-49db-93a3-59604a46a3b7', url: 'https://github.com/Edward-devops/Pipeline.git'
            }
        }

           stage('build') 
        {
            steps {
                echo "intergration test success"
               bat 'build.bat'
            }
        }
        
   stage('unitestcase') 
        {
            steps {
                echo "intergration test success"
               bat 'unitestcase.bat'
            }
        }
        
   stage('qualitycheck') 
        {
            steps {
                echo "intergration test success"
               bat 'qualitycheck.bat'
            }
        }
         stage('deploy') 
        {
            steps {
                echo "intergration test success"
               bat 'deploy.bat'
            }
        }
    }
}
