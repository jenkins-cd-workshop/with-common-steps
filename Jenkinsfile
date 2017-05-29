node {
    stage "Checkout", {
        checkout scm
    }
    
    stage "Update a file", {
        sh "echo 'some text' >> hello.txt && git add hello.txt"
    }
    
    stage "Showing diff", {
        echo gitDifferences()
    }
}
