node { 
    stage('Build') {
        checkout scm
        sh("ls -alh")
        sh("bin/build")
    }

    stage("Archive") {
        archiveArtifacts artifacts: demo-app*.tgz, fingerprint: true
    }
}