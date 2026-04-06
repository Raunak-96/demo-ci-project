node {

    stage('Checkout Code') {
        checkout scm
    }

    stage('Read File') {
        def content = readFile('raunak.txt')
        echo "File Content:\n${content}"
    }

    stage('Line Count') {
        def content = readFile('raunak.txt')
        def lines = content.split("\n")
        echo "Total Lines: ${lines.size()}"
    }

    stage('Word Check') {
        def content = readFile('raunak.txt')

        if(content.contains("city")) {
            echo "✅ Word 'city' found"
        } else {
            error "❌ Word 'city' NOT found → Build Failed"
        }
    }

}