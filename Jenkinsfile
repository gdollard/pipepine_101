@Library("shared-library") _

pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                // call a function from the shared-library
                helloWorld(name: "Mr Blobby", dayOfWeek: "Saturday");
            }
        }
    }
}