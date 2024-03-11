pipeline {
    agent any
    
    parameters {
    booleanParam description: 'specify if the job is done', name: 'true'
    choice choices: ['Cameroon', 'Nigeria', 'America', 'Ghana', 'France'], 
    description: 'My country of origin',
    name: 'country'
    string defaultValue: 'pinneaple and orange', 
    description: 'my preferred meal',
    name: 'fruit'
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                sh '''
                echo "It's $true that the struggle is over. I am originally from $country and my preferred meal is $fruit"
                '''
            }
        }
    }
}
