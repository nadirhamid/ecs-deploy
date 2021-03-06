# ECS deploy using Github Actions

This action deploys ECS services using [fabfuel/ecs-deploy](https://github.com/fabfuel/ecs-deploy) script.

## Example usage

```yml
uses: brunocascio/ecs-deploy@v1.2.0
with:
  access_key: awsAccessKey
  secret_key: awsSecretKey
  region: awsRegion
  cluster: theClusterName
  service: theServiceName
  task: theTaskDefinitionName
  container: theContainerName
  envfile: /path/to/your/envfile (optionally)
  timeout: 720 (optionally, default 300)
```
