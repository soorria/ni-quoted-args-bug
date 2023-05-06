To see the issue with quoted args, clone this repo and run

```sh
nr print "a b" 'c d' e
```

Output at time of writing this:

```js
[ 'a', 'b', 'c', 'd', 'e' ]
```

Expected output:

```js
[ 'a b', 'c d', 'e' ]
```

which matches what you get when you run

```sh
npm run print "a b" 'c d' e
```
