node {
    stage "Checkout", {
        checkout scm
    }
    
    stage "Update a file", {
        sh "echo 'some text' >> hello.txt && git add hello.txt"
    }
    
    stage "Showing diff", {
        if (gitDifferences()) {
            echo "Some differences we could open a pull request with..."
        } else {
            echo "Nothing interesting has been updated."
        }
    }
}
