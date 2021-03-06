Building
--------

```sh
# Dependencies
bower install
npm install --only=dev

# Build
npm run build
```

Running
-------

```sh
# index.html is a container for the actual page. For live reload.
open index.html

# Automatic rebuild. Live reload.
npm run dev
```

Sometimes you wanna open the page in a different device (like a mobile device).

```sh
# Serve the index.html
python -m SimpleHTTPServer
```

Then, point your device's browser to your host. To open the page directly (no container, no live reload), go to `<host>/build`.

Deploying
---------

```sh
# Be at the right place
cd kalabasa.github.io
git checkout src

# Deploy build
./deploy.sh
```
