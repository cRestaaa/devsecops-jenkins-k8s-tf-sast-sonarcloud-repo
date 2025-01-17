pipeline {
  agent any
  tools { 
        maven 'Maven_3.2.5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {
                sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecuritygurubuggy -Dsonar.organization=asecuritygurubuggy -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=e33907cc6ce92ad9ea03d2d0dc484fbbecb3488b'
                        }
        } 
  }
}
