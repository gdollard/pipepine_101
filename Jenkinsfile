@Library("shared-library-api-global-lib") _

// this pipeline will use shared libraries
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                script {
                    // call a function from the shared-library
                    helloWorld.sayHello(name: "Mr Blobby", dayOfWeek: "Saturday")
                    helloWorld.saySomethingElse("Goodbye")
                }
            }
        }
    }
}