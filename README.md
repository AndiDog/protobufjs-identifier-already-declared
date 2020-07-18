# pbts "Identifier 'end2' has already been declared" issue

```text
$ npm run build-proto

> protobuf-identifier-already-declared@0.0.0 build-proto /Users/[snip]/protobuf-identifier-already-declared
> rm -f src/proto.js && pbjs --es6 -t static-module -w es6 -o src/proto.js proto/Example.proto && pbts -o src/proto.d.ts src/proto.js

ERROR: Unable to parse /Users/[snip]/protobuf-identifier-already-declared/src/proto.js: Identifier 'end2' has already been declared (151:24)
/Users/[snip]/protobuf-identifier-already-declared/node_modules/protobufjs/cli/pbts.js:133
                throw err;
                ^

Error: code 1
    at ChildProcess.<anonymous> (/Users/[snip]/protobuf-identifier-already-declared/node_modules/protobufjs/cli/pbts.js:130:27)
    at ChildProcess.emit (events.js:327:22)
    at maybeClose (internal/child_process.js:1051:16)
    at Process.ChildProcess._handle.onexit (internal/child_process.js:287:5)
npm ERR! code ELIFECYCLE
npm ERR! errno 1
npm ERR! protobuf-identifier-already-declared@0.0.0 build-proto: `rm -f src/proto.js && pbjs --es6 -t static-module -w es6 -o src/proto.js proto/Example.proto && pbts -o src/proto.d.ts src/proto.js`
npm ERR! Exit status 1
npm ERR!
npm ERR! Failed at the protobuf-identifier-already-declared@0.0.0 build-proto script.
npm ERR! This is probably not a problem with npm. There is likely additional logging output above.

npm ERR! A complete log of this run can be found in:
npm ERR!     /Users/asommer/.npm/_logs/2020-07-18T06_45_39_202Z-debug.log
```
