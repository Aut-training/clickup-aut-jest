# clickup-aut-jest
PoC for Clickup application with jest framework 

### Edge support
1. In order to run the tests in Edge use **puppeteer-core** in the test file.

```javascript
const puppeteer = require('puppeteer-core');
```
2. Add **executablePath** property to **puppeteer.launch()** method.
```javascript
browser = await puppeteer.launch(
      {
        headless: false,
        args: ['--start-maximized'],
        executablePath: 'C:\\Program Files (x86)\\Microsoft\\Edge\\Application\\msedge.exe'
      }
    );
```
