pipeline{
    agent any 

    stages{
        stage('first'){
            steps{
                echo "first stage job"
                sh 'pwd'
            }
        }
        stage('two'){
            steps{
                echo "secong stage job"
                sh 'whoami'
            }
        }
    }
}