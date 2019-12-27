node('jenkins-slave') {
    stage ('Compile Stage') {
        container('maven') {
            sh 'mvn -B clean install'
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
