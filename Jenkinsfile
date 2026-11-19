
pipeline {
    agent any

    parameters {
        choice(
            name: 'BRANCH',
            choices: ['main', 'branch1', 'branch2', 'branch3'],
            description: 'Select the branch'
        )
    }

    stages {
        stage('Execute Branch') {
            steps {
                script {
                    if (params.BRANCH == 'branch1') {
                        echo 'Executing branch1'
                    }
                    else if (params.BRANCH == 'branch2') {
                        echo 'Executing branch2'
                    }
                    else if (params.BRANCH == 'branch3') {
                        echo 'Executing branch3'
                    }
                    else if (params.BRANCH == 'main') {
                        echo 'Executing main'
                    }
                }
            }
        }
    }
}
