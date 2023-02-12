![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT9ZJeGD2uuMbMmou--uIsn_lohzt4ZlOmovQ&usqp=CAU)
# how to use Router
```php
// controller classes
Route::get('/post/comment/{id}', 'Post@comment');
Route::get('/home', 'PostController@home');
Route::post('/login', 'Login@index');
Route::post('/register', 'Register@index')
```

```php
// callable method 
Route::get('/', function () {
echo "<div>page uri is : /</div>";
});
Route::get('/post/{id}/{name}', function ($data) {
echo $data['id'] . " :name= " . $data['name'];
});
```


* page not found class value = 'notFound'
* method value = 'index'
* can you change this value 
```php
Route::$NotFoundFun = 'notfoundpage1';
Route::$NotFoundClass = '404';
```

[]
