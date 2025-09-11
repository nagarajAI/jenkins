pipeline{
    agent any 

    parameters{
        string(name:"NAME", defaultValue:"admin", description:"Enter user name")
        booleanParam(name:"DEBUG", defaultValue:false, description:"ON/OFF debug mode")
        choice(name:"CHOICES", choices:['apple','orange','banana'])
    }

    stages{
        stage('first'){
            steps{
                echo "first stage job"
                sh 'pwd'
                echo "$NAME"
                echo "DebugMode: $DEBUG"
                sh 'sleep 10'
            }
        }
        stage('two'){
            steps{
                echo "secong stage job"
                sh 'whoami'
                echo "$CHOICES selected."
                sh 'sleep 10'
            }
        }
    }
}