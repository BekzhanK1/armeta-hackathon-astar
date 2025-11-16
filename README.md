# Armeta Hackathon Astar

This repository contains the complete Armeta Hackathon project, organized as a monorepo with git submodules.

## Structure

This repository uses git submodules to manage three separate components:

- **backend** - Backend service ([innovateX](https://github.com/dimalbek/innovateX.git))
- **frontend** - Frontend application ([Armeta-hackaton](https://github.com/AlikhanNasa7/Armeta-hackaton))
- **models-microservice** - Models microservice ([models_armeta](https://github.com/BekzhanK1/models_armeta.git))

## Getting Started

### Cloning the Repository

To clone this repository with all submodules:

```bash
git clone --recurse-submodules https://github.com/BekzhanK1/armeta-hackathon-astar.git
```

If you've already cloned the repository without submodules:

```bash
git submodule update --init --recursive
```

### Updating Submodules

To update all submodules to their latest commits:

```bash
git submodule update --remote
```

### Working with Submodules

Each submodule is an independent git repository. To work on a specific submodule:

```bash
cd backend  # or frontend, or models-microservice
# Make your changes
git add .
git commit -m "Your commit message"
git push
# Then go back to the main repo and commit the submodule reference update
cd ..
git add backend
git commit -m "Update backend submodule"
git push
```

