# Docker to ECS

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

```
## Reference

- [Yelb Posting](https://aws.amazon.com/ko/blogs/containers/deploy-applications-on-amazon-ecs-using-docker-compose/)
- [Yelb Project](https://github.com/mreferre/yelb)
- [Docker Docs](https://docs.docker.com/cloud/ecs-integration/)
