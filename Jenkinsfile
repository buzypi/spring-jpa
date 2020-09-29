pipeline {
  agent any
  stages {
    stage('Run Build') {
      steps {
        sh './mvnw clean install'
      }
    }

    stage('Archive Artifacts') {
      steps {
        archiveArtifacts 'target/demo-0.0.1-SNAPSHOT.jar'
      }
    }

  }
}