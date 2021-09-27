node {
    checkout scm

    docker.withRegistry('https://hub.docker.com/', 'DockerHub') {

        def customImage = docker.build("ameniii/test_evoli")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
