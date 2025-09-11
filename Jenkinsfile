pipeline{
    agent any 

    parameters{
        string(name:"NAME", defaultValue:"admin", description:"Enter user name")
        booleanParam(name:"DEBUG", defaultValue:false, description:"ON/OFF debug mode")
    }
    stages{
        stage('first'){
            steps{
                echo "first stage job"
                sh 'pwd'
                echo "$NAME"
                echo "DebugMode: ${param.DEBUG}"
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