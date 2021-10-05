# Ghost Update
A short script to updated and restart ghost to the version specified. This is for [Ghost](https://github.com/TryGhost/Ghost).

Restarts ghost using [appleboy's ssh action](https://github.com/appleboy/ssh-action).

To use this action, please copy and paste the action.yml file into your own workflows folder, and insert your secrets accordingly.
 
For the secrets,

  `SSH_HOST` refers to the host IP address/hostname.
  
  `SSH_USER` refers to the user. user@host.ip
  
  `PORT` refers to the port number you connect to your host at.
  
  `PATH_TO_GITHUB_REPO` refers to the folder you have your ghost code hosted. For me, this is different from the root ghost folder.
  
  `PATH_TO_GHOST` refers to the root folder of your ghost install on your server.
  
  `GIT_PULL_SCRIPT` is just `git pull token@github.com/repo`. See this [Stack Overflow answer](https://stackoverflow.com/questions/61447350/automatically-pull-from-remote-using-github-actions) for more details.
  
This was tested on DigitalOcean running Ubuntu 20.04
