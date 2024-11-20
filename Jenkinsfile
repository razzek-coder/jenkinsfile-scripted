node('jdk21') {
  def mvnHome
  try {
    stage('Stage1') {
      mvnHome = tool 'maven 3.9.9'
      echo 'Ejecucion stage 1'
    }
    stage('Stage2') {
      bat "${mvnHome}/bin/mvn" + ' --version'
    }
    stage('Stage3') {
      echo 'Ejecucion stage 3'
    }
  } finally {
    echo 'al final'
  }
}
