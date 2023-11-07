# first method

## create a HtmlMinifier.php file in the middleware folder of the application or download and move html minifier to middleware

## Register the HtmlMinifier.php in app\Https\Kernel.php file inside routeMiddleware
``htmlMinifier => app\Http\middleware\HtmlMinifier::class,``

## use htmlMinifier to wrap all routes in the application route file (web.php file)
```Route::middleware(['HtmlMinifier'])->group(function () {.....});```

## inspect the html Page using Google chrome or any browser that supports a developer tool
`` Ctrl + i ``



# 2nd method
