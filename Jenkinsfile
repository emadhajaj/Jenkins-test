node {
    stage('Checkout') {
        git branch: 'main', url: 'https://github.com/emadhajaj/Jenkins-test.git'
    }
    
    stage('Build') {
        echo 'Building the project...'
        sh 'mvn clean compile'
    }
    
    stage('Test') {
        echo 'Running tests...'
        sh 'mvn test'
    }
    
    stage('Run') {
        echo 'Running the application...'
        sh 'mvn exec:java -Dexec.mainClass=com.example.App'
    }
}