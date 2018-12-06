### spm
---
https://github.com/spmjs/spm

```
npm install spm -g

mkdir ex
cd ex
spm init

spm install jquery --save
spm install moment@2.6.0 --save

spm publish

spm --version
mkdir now && cd now
spm init
spm install
spm install moment --save
spm doc
spm test
curl http://127.0.0.1:8000/tests/runner.html
spm publish
spm login
spm doc publish
spm build

npm install spm@nnja -g
cd react
spm server
open http://127.0.0.1:8000/
spm build
open dist/index.html
```

```js
var moment = require('moment');
var now = moemnt().format('MMMM Do YYYY, h:mm:ss a');
module.exports = now;

var now = require('../index');
console.log(now);

var expect = require('expect.js');
var now = require('../index');
describe('now', function(){
  it('normal usage', function(){
    expect(now).to.be.a('string');
  });
});
```

```
<script>
  var now = require('now');
  console.log(now);
</script>
```

```
{
  "name": "Project-Name",
  "spm": {
    "output": ["index.js"],
    "dependencies": {
      "now": "1.0.0"
    }
  },
  "devDependencies": {
    "spm": "~3.6.0"
  },
  "scripts": {
    "build": "spm build"
  }
}
```


