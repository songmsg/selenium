pipeline {
    environment {
        MAILCATEGORIZER = '[Jenkins]'
        RECIPIENTS_FAILURE = 'extern.song_wenying@allianz.com'
        RECIPIENTS_UNSTABLE = 'extern.song_wenying@allianz.com'
        RECIPIENTS_SUCCESS = 'extern.song_wenying@allianz.com'
        RECIPIENTS_ALWAYS = 'extern.song_wenying@allianz.com'
    }
    agent { label 'maven' }
    stages {
        stage('Run Tests') {
            steps {
                sh 'mvn clean test'
            }
        }
    }
}