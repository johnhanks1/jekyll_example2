pipeline {
  agent any
    stages {
      stage('Build') {
        steps {
          awsCodeBuild projectName: 'runthrough',
                       credentialsId: 'pipelineExample',
                       credentialsType: 'jenkins',
                       region: '#{region}',
                       sourceControlType: 'jenkins'

        }
      }
    }
}
