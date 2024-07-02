# Launcher

This is the launcher for all the microservices of the project. It is a simple script that starts all the services in the correct order.

## How to use

1. Clone the repository
2. Run `git submodule update --init --recursive` to clone all the submodules
3. Run `docker compose up --build` to start all the services

## How to add a new submodule

1. Run `git submodule add <repository-url> <path>` to add the submodule
2. Add the changes to the main repository with

```bash
git add .
git commit -m "Add <submodule-name> submodule"
git push
```

3. Run `git submodule update --init --recursive` to clone the submodule
4. Run `git submodule update --remote --recursive` to update the submodule

### Disclaimer

Make the commit of the submodule in the main repository before updating the submodule. This way, the main repository will have the correct reference to the submodule.
