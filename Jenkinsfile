node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'docker-creds') {

        def customImage = docker.build("sandeesh/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
