pipeline {
    agent any
    stages {
        stage('Clone') { steps { checkout scm } }
        stage('Build') { steps { echo 'Building...'; sh 'mkdir -p out && echo "done" > out/hi.txt' } }
        stage('Archive') { steps { archiveArtifacts 'out/*.txt' } }
    }
}
