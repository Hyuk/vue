# Vue Basics
* {}
* v-text
* v-html

## {}
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Hello vue.js</title>
    <script src="https://cdn.jsdelivr.net/npm/vue@2.5.21/dist/vue.js"></script>
</head>
<body>
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
</body>
</html>
```

## v-text
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Hello vue.js</title>
    <script src="https://cdn.jsdelivr.net/npm/vue@2.5.21/dist/vue.js"></script>
</head>
<body>
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
</body>
</html>
```

## v-html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Hello vue.js</title>
    <script src="https://cdn.jsdelivr.net/npm/vue@2.5.21/dist/vue.js"></script>
</head>
<body>
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
</body>
</html>
```