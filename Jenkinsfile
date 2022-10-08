pipeline {
        agent any
        stages{
                stage('build'){
                        steps{
                                sh 'docker build -t belajar .'
                        }
                }
                stage('run'){
                        steps{
                                sh 'docker run --name belajar -d -p 5000:80 belajar'
                        }
                }

                // stage('clean up'){
                //         steps{
                //                 sh 'docker stop belajar-pipeline-3 || true'
                //                 sh 'docker rm belajar-pipeline-3 || true'

                //         }
                // }
        }
}