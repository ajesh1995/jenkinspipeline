pipeline {
    agent any
  parameters {
  choice choices: ['dev', 'prod', 'sit'], description: 'select environment', name: 'ENV'
}
environment {
  JAVA_HOME = "/usr/bin/java8"
}

    stages {
        stage ("welcome") {
            steps {
                script {
                    // printing default variables 
                    println "BUILD_NUMBER is ${BUILD_NUMBER}"
                    println "WORKSPACE is ${WORKSPACE}"

                    // printing the values of parameters
                    println "selected env is ${params.ENV}"
                }
            }
        }
    }
}
