# dev_JenkinsCICDPipeline
Jenkins CI CD Pipeline Development

#### Pipeline as Code
[https://plugins.jenkins.io/workflow-aggregator/](https://plugins.jenkins.io/workflow-aggregator/) <br/>

##### Pipeline as Code Github Demo
[https://hub.docker.com/r/jenkinsci/pipeline-as-code-github-demo/](https://hub.docker.com/r/jenkinsci/pipeline-as-code-github-demo/) <br/>


##### Writing Pipeline-Compatible Plugins
[https://www.jenkins.io/doc/developer/plugin-development/pipeline-integration/](https://www.jenkins.io/doc/developer/plugin-development/pipeline-integration/) <br/>


#### Build Flow plugin (deprecated)
[https://wiki.jenkins.io/display/JENKINS/Build+Flow+Plugin](https://wiki.jenkins.io/display/JENKINS/Build+Flow+Plugin) <br/>


#### Docker Workflow Demo
[https://hub.docker.com/r/jenkinsci/docker-workflow-demo/](https://hub.docker.com/r/jenkinsci/docker-workflow-demo/) <br/>

#### Jenkins CI/CD Template
Create Jenkins Pipeline <br/>
![Jenkins Pipeline](https://github.com/lel99999/dev_JenkinsCICDPipeline/blob/main/JenkinsCICd-01.PNG) <br/>

Script directly or upload Jenkinsfile: <br/>

```
pipeline {
   agent any

   stages {
      stage('Build') {
        steps {
          echo 'Building...'
          echo "Running ${env.BUILD_ID} ${env.BUILD_DISPLAY_NAME} on ${env.NODE_NAME} and JOB ${env.JOB_NAME}"
        }
   }
   stage('Test') {
     steps {
        echo 'Testing...'
     }
   }
   stage('Deploy') {
     steps {
       echo 'Deploying...'
     }
   }
  }
}
```

#### Docker Demo
[https://hub.docker.com/r/jenkinsci/pipeline-as-code-github-demo](https://hub.docker.com/r/jenkinsci/pipeline-as-code-github-demo) <br/>

View Log:
```
$docker container ls
$docker logs --details <container_id>
```
