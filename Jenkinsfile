node {
    checkout scm

    docker.withRegistry('https://hub.docker.com/', 'DockerHub') {

        def customImage = docker.build("ameni/testevoli")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
