node{
    git branch: 'main', url: 'https://github.com/emadhajaj/Jenkins-test.git'
    
    // Set Java 21 as the runtime
    env.JAVA_HOME = tool 'Java21'
    
    stage('Checkout') {
        checkout scm
    }

    stage('Build') {
        sh 'echo Building with Java 21...'
        sh 'mvn clean compile'
    }

    stage('Test') {
        sh 'echo Testing...'
        sh 'mvn test'
    }

    stage('Deploy') {
        sh 'echo Deploying...'
        // Add your deploy commands here
    }
}