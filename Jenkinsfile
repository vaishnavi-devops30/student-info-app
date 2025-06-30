pipeline {
  agent any

  tools {
  maven 'Maven 3.9.9'
  jdk 'JDK 21'
}


  stages {
    stage('Build') {
      steps {
        sh 'mvn clean compile'
      }
    }

    stage('Run') {
      steps {
        sh 'java -cp target/classes com.devops.student.StudentInfoApp'
      }
    }
  }
}

