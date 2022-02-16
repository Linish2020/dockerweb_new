node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'armor') {

        def customImage = docker.build("linish/node-web-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}