node{
    git branch: 'main', url: 'https://github.com/emadhajaj/Jenkins-test.git'

    
    stage('build') {
        try {
        sh 'echo "build stage"'
        }
        catch(Exception e) {
            sh 'echo "build failed"'
            throw e
        }
    }

    stage('Test') {
        if (env.BRANCH_NAME == 'feat') {
            sh 'echo "Test stage on main branch"'
        
        } else {
            sh 'echo "skipping Test stage on non-main branch"'
        }
    }

}