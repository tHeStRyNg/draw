### Draw

Open Source fork from excalidraw

#### Install

- Install Yarn -> https://linuxize.com/post/how-to-install-yarn-on-ubuntu-20-04/

```nvm use``` # there is a .nvmrc that you can use ^_^

```yarn``` # Installs Dependencies
```yarn start``` Starts the App

#### Troubleshooting

- Error: ENOSPC: System limit for number of file watchers reached

```echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p```
