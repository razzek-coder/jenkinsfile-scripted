node('jdk21') {
  def mvnHome
  try {
    stage('Stage1') {
      mvnHome = tool 'maven 3.9.9'
      echo 'Ejecucion stage 1'
    }
    stage('Stage2') {
      try {
        bat "${mvnHome}/bin/mvn" + ' --version'
      } finally {
        echo 'dentro de stage 2'
      }
    }
    stage('Stage3') {
      echo 'Ejecucion stage 3'
    }
  } finally {
    echo 'al final'
  }
}
