node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com/', 'DockerHub') {

        def customImage = docker.build("ildikom/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}