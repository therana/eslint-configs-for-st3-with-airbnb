## Installation of Eslint with Airbnb and some initial configs.

### Installation Process of required plugins on Sublime Text
Before installation make sure you have installed `'SublimeLinter'` & `'Sublime​Linter-contrib-eslint'` via package control.

  ```sh
  npm install -g eslint
  npm info "eslint-config-airbnb@latest" peerDependencies
  (
  export PKG=eslint-config-airbnb;
  npm info "$PKG@latest" peerDependencies --json | command sed 's/[\{\},]//g ; s/: /@/g' | xargs npm install -g "$PKG@latest"
)
  ```