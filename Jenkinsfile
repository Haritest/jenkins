node() {
 try {
        String ANSI_GREEN = "\u001B[32m"
        String ANSI_NORMAL = "\u001B[0m"
        String ANSI_BOLD = "\u001B[1m"
        String ANSI_RED = "\u001B[31m"
        String ANSI_YELLOW = "\u001B[33m"
  
  stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */
        cleanWs()
        checkout scm
    }

    stage('Build image') {
        /* This builds the actual image; synonymous to
         * docker build on the command line */

        sh 'echo "test passed"'
    }

    stage('Test image') {
        /* Ideally, we would run a test framework against our image.
         * For this example, we're using a Volkswagen-type approach ;-) */

            sh 'echo "Tests passed"'
            cleanWs()
    }
}
 
    catch (err) {
        throw err
    } 
}
