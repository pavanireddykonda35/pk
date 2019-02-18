node{
    stage('build now') {
git ' https://github.com/pavanireddykonda35/pk.git'
    }
    stage('build mvn') {
sh 'mvn package'
    }
    stag('test result') {
    junit 'target/*surefire-reports/*.xml'
    }
    stage( 'archifacts') {
        archiveArtifacts 'target/*.jar'
    }
}
