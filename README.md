# lern-vuejs
lerning vuejs

## install command 

```
nvm use 18.16.1
npm install yarn -g 

npm install -g @vue/cli
# OR
yarn global add @vue/cli

vue create hello-world
cd hello-world/
yarn serve
```


## other command 

```bash
nvm install 18.16.1
nvm install 16.20.2
# OR
nvm uninstall 18.16.1
nvm uninstall 16.20.2
```

## pm2 start ecosystem.config.json

ecosystem.config.json

```json
{
  "apps": [
    {
      "name": "my-app",
      "script": "npm",
      "args": "run dev",
      "cwd": "./",
      "instances": 1,
      "exec_mode": "fork",
      "autorestart": true,
      "watch": false,
      "max_memory_restart": "500M",
      "env": {
        "NODE_ENV": "development"
      },
      "env_production": {
        "NODE_ENV": "production"
      }
    }
  ]
}
```
