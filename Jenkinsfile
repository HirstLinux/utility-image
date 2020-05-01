node {
    checkout scm
    docker.withRegistry('https://registry.hub.docker.com', 'hirstlinux-docker') {
        def customImage = docker.build("hirstlinux-utility-image:${env.BUILD_ID}")
        customImage.push()
    }
}