# Inlaze

Full stack technical test development for Inlaze

## Backend dev

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

4. copy `.env.template` and rename to `.env`

5. builds and run Docker images for all services defined in the `docker-compose.yml` file and then starts the containers.

```
docker compose up --build
```

You can use the seed for authentication by making a request in:

`http://localhost:3000/api/docs#/auth/AuthController_seed`

## Frontend dev

1. Enter the frontend folder with `cd ./frontend`

2. copy `.env.template` and rename `.env`

3. install dependencies

```
npm install
```

```
yarn install
```

3. run application

```
npm run dev
```

### Add submodule

Add the submodule, where `repository_url` is the repository URL and `directory_name` is the folder name where you want to store the submodule (must not exist in the project)

```
git submodule add <repository_url> <directory_name>
```
