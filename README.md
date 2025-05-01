# micosaas_starter
This creates boiler plate starter components for a microsaas project


## Docker
### Running Docker
docker-compose up --build

### Stopping Docker Service
docker-compose up

### cloning repo with submodules
git clone --recursive https://github.com/yourusername/landing-ai.git

### update submodules
git submodule update --init --recursive


### Issues with Gitmodules
## Remove all submodules
git submodule deinit -f --all

### Remove the .git/modules directory
rm -rf .git/modules

### Re-add both submodules
git submodule add https://github.com/jileyitayo/landingpage_ai_frontend.git frontend
git submodule add https://github.com/jileyitayo/landingpage_ai_backend.git backend



// ...existing code...

## Version Management

### Creating Tags Across Repositories
```bash
# Tag submodules
cd frontend
git tag -a v1.0.0 -m "Initial frontend release v1.0.0"
git push origin v1.0.0

cd ../backend
git tag -a v1.0.0 -m "Initial backend release v1.0.0"
git push origin v1.0.0

# Tag main repository
cd ..
git tag -a v1.0.0 -m "Initial release v1.0.0"
git push origin v1.0.0
```

### Checking Out Specific Version
```bash
# Checkout main repo version
git checkout v1.0.0

# Update submodules to their corresponding tags
git submodule update --recursive
```