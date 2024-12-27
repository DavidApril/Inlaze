# Inlaze

Full stack technical test development for Inlaze

## Development

1. Clone the repository to your local machine

```
git clone https://github.com/sftCommunity/microservices.git
```

2. Initialize and update submodules when someone clones the repository for the first time, they must execute the following command to initialize and update the submodules

```
git submodule update --init --recursive
```

3. To update submodule references

```
git submodule update --remote
```

5. builds and run Docker images for all services defined in the `docker-compose.yml` file and then starts the containers.

```
docker compose up --build
```

### Add submodule

Add the submodule, where `repository_url` is the repository URL and `directory_name` is the folder name where you want to store the submodule (must not exist in the project)

```
git submodule add <repository_url> <directory_name>
```
