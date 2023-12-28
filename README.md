# pm2-guide
A Basic pm2 guide :)


# Usage
Download the bots and node modules you want to use by pressing the SHIFT + MOUSE RIGHT shortcut.
Then create the ecosystem.config.js file, briefly as follows:

![image](https://github.com/takachim/pm2-guide/assets/109786377/2c7dd98d-28e4-456d-813e-f98f36bb79be)


Then what you need to do is to specify the main files of the folders in the ecosystem.config.js file, as follows.
```js
module.exports = {
    apps: [
        {
            name: "takachi-ai",
            namespace: "AI",
            script: 'takachi', //main file
            watch: false,
            exec_mode: "cluster",
            max_memory_restart: "500M",
            cwd: "./takachi-ai" //file path
          },
    ]
}
```

# Runing System
If all your config and systems are ready, open CMD using the SHIFT + MAUSE RIGHT shortcut in the folder where the bots are located and
Create a clean package.json file with the npm init -y command.
Then type npm i pm2@latest -g -s after the download is completed.
It will be enough to type pm2 start.

![image](https://github.com/takachim/pm2-guide/assets/109786377/6976ebea-245e-4071-996c-9f6b8926e9d6)

# Closing the system
If you want to close the sistem just use pm2 kill command.

# How to see the logs?
To view the logs in PM2, open CMD using the SHIFT + MAUSE RIGHT shortcut on the desktop.
and then type the pm2 logs command.
![image](https://github.com/takachim/pm2-guide/assets/109786377/90a2fefb-f71f-4bb1-ba73-f30b7f90b408)


# Contact me

[![Discord Presence](https://lanyard.cnrad.dev/api/149284207833645056)](https://discord.com/users/149284207833645056)
