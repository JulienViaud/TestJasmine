node {
    env.NODEJS_HOME = "${tool 'Node 8.9.1'}"
    // on linux / mac
    // env.PATH="${env.NODEJS_HOME}/bin:${env.PATH}"
    // on windows
    env.PATH="${env.NODEJS_HOME};${env.PATH}"
    sh 'npm --version'
    
    stage('DL') {
      checkout scm
      sh 'npm install'
    }

    stage('Test') {
      sh 'npm test'
    }
}
© 2017 GitHub, Inc.
