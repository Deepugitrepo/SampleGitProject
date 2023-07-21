pipeline{
  tools{
    maven 'Maven'
  }
  agent any
  stages {
    stage ('Initialize'){
      sh '''
            echo "PATH = ${PATH}"
            echo "M2_HOME = ${M2_HOME)"
      '''
    }

    stage ('Build'){
      sh 'mvn clean package'
    }
  
  }
  
  
}
