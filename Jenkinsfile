pipeline{
  tools{
    maven 'Maven'
  }
  agent any
  stages {
    stage ('Initialize'){
      steps {
        sh'''
              echo "Initializing..."
              echo "PATH = ${PATH}"
              echo "M2_HOME = ${M2_HOME}"
        '''
      }
    }

    stage ('Build'){
      steps{
        sh 'mvn clean package'
      }
    }
  
  }
  
  
}
