<h1 align="center">
 Docker File from php8.2  <br>
 (Laravel, Symfony, Wordpress, etc..)
</h1>

<p align="center">
    <img src="https://gridcp.com/wp-content/uploads/2021/04/logo-gridcp-rrss-1024x538.png">	
</p>


![Packagist PHP Version Support](https://img.shields.io/badge/php-%5E8.2-blue)


Docker file for use in PHP Symfony support for php 8.2.
- Laravel
- PhpCake.
- Wordpress.
- Drupal.
- etc.




## 🚀 Installation
### From Docker File.

In your terminal in same folder you down dockerfile execute this sentences.
```terminal
docker build -t gridcp/gridcp-php-fpm82 .
docker run -p 9000:9000  --name gridcp_php82 gridcp/gridcp-php-fpm82 
```

## :arrow_forward: How to use.
In your web server to use this container add the proxy pass for example:.
### Apache.
```conf
ProxyPassMatch ^/(.*\.php(/.*)?)$ fcgi://gridcp_php82:9000/var/www/html/public/$1
```

## :mag_right: Change log
Please see <a href="https://github.com/GridCP/docker-php-8.5.2/blob/main/changelog.md">CHANGELOG</a> for more information what has changed recently.



## :superhero_woman: Contribute.
Feel free to make as many pull requests as you think fit, because there are so many things to do, all help is welcome.

Here is a guide if you want to take a look()

If you find a bug, let us know <a href="https://github.com/GridCP/docker-php-8.5.2/issues">here</a> .

If you request a new  <a href ="https://github.com/GridCP/docker-php-8.5.2/issues"> feature</a>.
