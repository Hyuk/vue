# {{}}, v-text, v-html 차이점

* {{}}와 v-text를 쓸때는 html 코드 <, >를 인코딩해서 나타낸다.
* v-html을 쓸때는 html 코드 <, >를 적용해서 나타낸다.

```html
<div id="simple">
    <h2>{{message}}</h2>    <!-- <i>첫 번째 Vue.js 앱입니다.</i> -->
    <h2 v-text="message"></h2>  <!-- <i>첫 번째 Vue.js 앱입니다.</i> -->
    <h2 v-html="message"></h2>  <!-- 첫 번째 Vue.js 앱입니다. (이탤릭 스타일)-->
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