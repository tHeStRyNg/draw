### Draw

Open Source fork from excalidraw

#### Install

- Server -> Debian fork ubt 20x

- Install Yarn 

``` curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - ```

``` echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list ```

``` sudo apt update ```

``` sudo apt install yarn ```

- The command above will also install Node.js . If you installed Node trough nvm, skip the Node.js installation with:

``` sudo apt install --no-install-recommends yarn ```

``` nvm use ``` # there is a .nvmrc that you can use ^_^

``` yarn ``` # Installs Dependencies

``` yarn start ``` Starts the App

#### Troubleshooting

- Error: ENOSPC: System limit for number of file watchers reached

``` echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p ```
