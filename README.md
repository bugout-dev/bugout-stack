# bugout-stack

## Running Bugout stack

Brood, Spire and Moonstream

### Installation and setup

To set up your environment for development, do the following:

- Clone the git repository and fetch all modules

```bash
git clone --recurse-submodules https://github.com/bugout-dev/bugout-stack.git
```

- Install Docker (https://docs.docker.com/engine/install/)
- Install Docker Compose (https://docs.docker.com/compose/install/)

#### Run Moonstream setup

- At first, prepare environment variables

```bash
./brood/configs/docker_generate_env.bash -d db_dev
./moonstream/backend/configs/docker_generate_env.bash -d db_dev
./moonstream/db/configs/docker_generate_env.bash -d db_dev
```

- Run containers with docker-compose

```bash
docker-compose up --build
```
