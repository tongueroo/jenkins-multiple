pipeline {
    agent {
        kubernetes {
            cloud 'kubernetes'
            label 'demo-gcp'
            yamlFile 'pod.yaml'
        }
    }

    stages {
        stage('Main') {
            steps {
            		build job: "test1"
            		build "test2"
            }
        }
    }
}
