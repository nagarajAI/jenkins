pipeline{
    agent any 

    parameters{
        string(name:"NAME", defaultValue:"admin", description:"Enter user name")
    }
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