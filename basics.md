# Vue Basics
* {{ }}
* v-text
* v-html
* v-bind
* v-model

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
* html코드를 적용하여 표시한다
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


## v-model
* 양방향 바인딩