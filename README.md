Running ClojureScript on OpenWhisk
==================================

Sample OpenWhisk action written in ClojureScript.

## Installing

First, compile ClojureScript

```bash
> lein cljsbuild once server-prod
```


 ```bash
 > npm install
 ```

This command installs the node modules and generates the source code for the action at `openwhisk-cljs-0.0.1.js`.

## Testing it locally

```bash
> node ./test/standalone.js 

  Loading:./openwhisk-cljs-0.0.1.js
  About to call ClojureScript. Wish me luck.
  { payload: 'Hello from greet' }
  About to call ClojureScript. Wish me luck.
  RESULT:
  { payload: 'Hello from greet' }
```
