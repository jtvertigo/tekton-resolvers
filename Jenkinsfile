pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                checkout scm
                tektonCreateRaw(input: ".tekton/hello-world.yml", inputType: "FILE", namespace: 'tekton-cicd')
            }
        }
    }
}