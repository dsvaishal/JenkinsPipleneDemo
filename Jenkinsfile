node {

       stage("Checkout")
       {
           checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '43999cd4-a961-4215-b532-60c38dfa9dde', url: 'https://github.com/dsvaishal/JenkinsPipleneDemo.git']]])
       }
       stage("Build")
       {
            bat """
            javac HelloWorld.java
            java HelloWorld
            """
       }
   
}
