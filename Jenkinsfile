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
            		build "test1", parameters: {FOO: "bar"}
            		build "test2"
            }
        }
    }
}
