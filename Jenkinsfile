pipeline {
    agent any

    stages {
        stage('Create File') {
            steps {
                sh '''
                    echo 'print("this is my pipeline")' > pipeline.py
                    cat pipeline.py
                '''
            }
        }

        stage('Run Python') {
            steps {
                sh 'python3 pipeline.py'
            }
        }
    }
}
