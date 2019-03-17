# [System JS issue 1914](https://github.com/systemjs/systemjs/issues/1914)

## Starting

* npm install
* npm start

## Cases

### src/simple.html

1. Loading fine1.js, THEN printing result
2. Loading error.js, CATCH printing error
3. Loading fine2.js, CATCH printing error
4. Showing System registry, where fine2.js equal error.js module

### src/workaround.html

1. Loading fine1.js, THEN printing result
2. Loading error.js, CATCH printing error
3. Deleting error.js from registry
4. Loading fine2.js, CATCH printing error
5. Showing System registry, where fine2.js equal error.js module

