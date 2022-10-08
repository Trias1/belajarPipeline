pipeline {
        agent any
        stages{
                stage('build'){
                        steps{
                                sh 'docker build -t belajar .'
                        }
                }

                stage('clean up'){
                        steps{
                                sh 'docker stop belajar || true'
                                sh 'docker rm belajar || true'

                        }
                }
               stage('run'){
                        steps{
                                sh 'docker run --name belajar -d -p 5000:80 belajar'
                        }
                }
        }
}