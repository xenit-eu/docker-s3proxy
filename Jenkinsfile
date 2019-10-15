node {
    stage("Checkout") {
        checkout scm
    }
    stage("Build Docker Image") {
        sh "./gradlew buildDockerImage"
    }
    stage("Push Docker Image") {
        sh "./gradlew pushDockerImage"
    }
}
