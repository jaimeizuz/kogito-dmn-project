pipeline {
    agent {
        docker {
            image 'jizuzquiza/kogito-quarkus-ci-builder-image:1.0.0_quarkus-2.16.9.Final'
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -Dorg.kie.dmn.runtime.typecheck=true clean package' 
            }
        }
    }
}