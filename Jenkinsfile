node('jenkins-slave') {
    stage ('Compile Stage') {
        container('maven') {
            sh 'mvn clean compile'
        }
    }

    stage ('Testing Stage') {
        container('maven') {
            sh 'mvn test'
        }
    }
    
    stage ('Deployment Stage') {
        container('maven') {
            sh 'mvn deploy'
        }
    }
}
