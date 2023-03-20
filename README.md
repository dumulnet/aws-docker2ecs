# Docker to ECS

- You docker compose up and Docker reads the docker-compose.yaml
- Docker converts the original compose file on the fly into an AWS CloudFormation template
- Docker deploys the CloudFormation template on AWS

## Quick Start
- Install Docker 19.03 or later or Docker Desktop for Mac
```
git clone https://<this_repo_url> 

//local test
docker-compose up

//aws configuration
aws config

//list current context
docker context ls

//create context for ecs
docker context create ecs myecscontext

//use ecs context
docker context use myecscontext

//convert docker-compose stack to cloudformation
docker compose convert

//Deployment to ECS
docker compose up

//Details of the compose stack -> Find the url of LB
docker compose ps
```
## Reference

- [Yelb Posting](https://aws.amazon.com/ko/blogs/containers/deploy-applications-on-amazon-ecs-using-docker-compose/)
- [Yelb Project](https://github.com/mreferre/yelb)
- [Docker Docs](https://docs.docker.com/cloud/ecs-integration/)
