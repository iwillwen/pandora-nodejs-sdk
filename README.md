# Pandora SDK for Nodejs

### 快速使用
```
npm install pandora-nodejs-sdk --save
// 或者
yarn add pandora-nodejs-sdk
```

```javascript

const { send, Auth } = require('./index')

const auth = new Auth(
  'your_ak',
  'your_sk'  
)

const points = [
  { name: 'foo', age: 23},
  { name: 'bar', age: 24}
]

send(auth, 'your_repoName',  points).then(
  () => console.log('success'),
  err => console.log(err)
) 

```