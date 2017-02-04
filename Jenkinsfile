node {
    checkout scm

    stage("Build") {
        sh("DOCKER_REGISTRY=armory arm build")
    }
    stage("Push Image") {
        sh("DOCKER_REGISTRY=armory arm push")
    }
}
