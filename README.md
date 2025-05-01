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