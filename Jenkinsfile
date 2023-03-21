@Library("shared-library-api-global-lib") _

// this pipeline will use shared libraries
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                script {
                    // call a function from the shared-library
                    hello.sayHello(name: "Mr Blobby", dayOfWeek: "Saturday")
                    hello.scanStuff(message: "Scanning folder for my pipeline", dirToScan: "lib")
                }
            }
        }
    }
}