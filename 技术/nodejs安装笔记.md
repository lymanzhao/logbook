tar -xvf "/opt/node-v11.6.0-linux-x64.tar.xz"

ln -s "/opt/node-v11.6.0-linux-x64/bin/npm" /usr/local/bin/

ln -s "/opt/node-v11.6.0-linux-x64/bin/node" /usr/local/bin/

npm install -g cnpm --registry=https://registry.npm.taobao.org

ln -s "/opt/node-v11.6.0-linux-x64/bin/cnpm" /usr/local/bin/

cnpm -v

cnpm install webpack -g

ln -s "/opt/node-v11.6.0-linux-x64/bin/webpack" /usr/local/bin/

webpack -v

cnpm install webpack-dev-server -g

webpack -dev-server -v

