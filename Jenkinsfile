//Hello! This is a new change!
node {
    // 1. Clone the repository
    stage('Clone Repository') {
        checkout scm
    }

    // 2. Build stage
    stage('Build') {
        echo 'Building the project...'
        sh 'mkdir -p build && echo "Scripted Build Success" > build/result.txt'
    }

    // 3. Echo Status and Archive
    stage('Archive Artifacts') {
        archiveArtifacts 'build/*.txt'
        echo "Build Status: SUCCESS"
    }
}
