https://cryptopage-vue.netlify.app/

The page initially seemed very easy to develop, as a result, 70% of the work had to be redone.
Difficulties arose at each stage:
- unable to scale images. Problem solved.
- it was necessary to create json and get data from it: done with fetch.
- it was necessary to implement drop-down blocks in the FAQ section - standard output method array in the loop was not suitable due to duplication of elements. Solution: pass an array object from App.vue to the FaqAnswers.vue component one by one, in the FaqAnswers.vue component, display the elements of the list through a loop.

# crypto-vue

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
