pipeline {
    agent any 
    stages {
        stage ("welcome") {
            steps {
                script {
                    var1 = input message: 'please enter a value', parameters: [string(defaultValue: '10', name: 'string1')]
                    println "my var1 value is ${var1}"
                }
            }
        }
    }
}
