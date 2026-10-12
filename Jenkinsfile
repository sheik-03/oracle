pipeline{
    agent any
    stages{
        stage("github"){
            steps{
                git credentialsId: 'hello_sheik', url: 'https://github.com/sheik-03/oracle.git'

            }

        }
        stage("build"){
            steps{
                'sh python3 --version'
                'sh echo successfully run in version'
            }
        }
        stage("test"){
            steps{
                'sh echo welcomme to the jenkins testing team'
            }
        }
        stage('deploy'){
            steps{
                'sh python3 app.py'
            }
        }
    }
}
