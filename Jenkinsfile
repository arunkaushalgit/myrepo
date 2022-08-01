pipeline {

  agent any

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')

  }

  stages {

    stage('Print Java') {

      steps {

        sh '''

          java -version

        '''

      }

    }
        stage('cat README') {
          steps {
            echo "hello arun"

      when {

        branch "source1"

      }

      steps {

        sh '''

          cat README.md

        '''

      }

    }


  }

}
