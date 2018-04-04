pipeline{
        agent any
        stages {
                stage('build')
                    {
                      steps {
                          sh ' mvn -X package '
                            }
                    }
               }
}
post {
        always{
                archive'/*.war'
        }
}
                
