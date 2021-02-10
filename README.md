## Audio Call via WebRTC: React Application for KaiOS

Based on: https://github.com/iurii-kyrylenko/peerjs-review

#### Create an empty npm project for local peer server:
```json
{
  "name": "peerjs-server",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "start": "peerjs --port 9000 --path /web-phone --allow_discovery"
  },
  "author": "",
  "license": "ISC",
  "dependencies": {
    "peer": "^0.6.1"
  }
}
```

#### Start peer server:
- `npm start`

#### Get peer list:
- `http://127.0.0.1:9000/web-phone/peerjs/peers`

#### Run application in dev mode:
- `yarn start`

#### Build application for deployment:
1. Edit file `src/config.js`
2. Run `GENERATE_SOURCEMAP=false yarn build`
3. Deploy `build` folder to the device.
