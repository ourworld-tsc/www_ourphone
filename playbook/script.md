```js
!!website.define 
    name:'www_ourphone_tf' 
    title:'Ourphone'

!!website.template_add url:'https://github.com/freeflowuniverse/webcomponents/tree/main/zola'
```

we need to import the content so that we can use it to build the website
```js
!!website.doctree_add url:'https://github.com/ourworldventures/www_ourphone/tree/development/content'
!!website.doctree_add url:'https://github.com/threefoldfoundation/threefold_data'
```

here we add the pages we need from content to the website.

```js
!!website.page_add 
    name: 'Ourphone'
    collection: 'content'
    file: 'ourphone.md'
    homepage: true

!!website.page_add
    name: 'Buy Now'
    collection: 'content'
    file: 'buy_now.md'

!!website.page_add
    name: 'Specs'
    collection: 'content'
    file: 'specs.md'
```

now lets add a blog section

```js
!!website.blog_add
    file: 'realizing_the_promise.md'
    collection: blog
```
