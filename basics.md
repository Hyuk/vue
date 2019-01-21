# Vue Basics
* {{ }}
* v-text
* v-html
* v-bind
* v-model
* v-show
* v-if, v-else, v-else-if

## {{ }}
* html코드를 인코딩하여 표시한다.
```html
<div id="simple">
    <h2>{{message}}</h2>
</div>
<script type="text/javascript">
var model = {
    message: '<i>첫 번째 Vue.js 앱입니다.</i>'
};

var simple = new Vue({
    el: '#simple',
    data: model
})
</script>
```

## v-text
* html코드를 인코딩하여 표시한다.
```html
<div id="simple">
    <h2 v-text="message"></h2>
</div>
<script type="text/javascript">
var model = {
    message: '<i>첫 번째 Vue.js 앱입니다.</i>'
};

var simple = new Vue({
    el: '#simple',
    data: model
})
</script>
```

## v-html
* html코드를 적용하여 표시한다.
```html
<div id="simple">
    <h2 v-html="message"></h2>
</div>
<script type="text/javascript">
var model = {
    message: '<i>첫 번째 Vue.js 앱입니다.</i>'
};

var simple = new Vue({
    el: '#simple',
    data: model
})
</script>
```

## v-bind
* 단방향 바인딩
* html코드를 인코딩하여 표시한다.
```html
<div id="simple">
    <input id="a" type="text" v-bind:value="message">
    <br />
    <img v-bind:src="imagePath" />
</div>
<script type="text/javascript">
var model = {
    message: '<i>v-bind 디렉티브</i>',
    imagePath: "https://avatars3.githubusercontent.com/u/1525621"
};

var simple = new Vue({
    el: '#simple',
    data: model
})
</script>
```

## v-model
* 양방향 바인딩
```html
<div id="simple">
    <input type="text" v-model="name" placeholder="Please type your first name">
    <br />
    <h2 v-html="name"></h2>
</div>
<script type="text/javascript">
var simple = new Vue({
    el: '#simple',
    data: {
        name: ''
    }
})
</script>
```

## v-show
* 렌더링 후 조건에 맞으면 display
```html

```