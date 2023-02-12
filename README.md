![](https://images.unsplash.com/photo-1599507593548-0187ac4043c6?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8M3x8cGhwfGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=1800&q=60)
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
