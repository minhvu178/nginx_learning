# nginx_learning
Introduction:
This is basically a module based on many other "hello_world" on the internet. Its purpose is nothing but trying to print out Hello World when request localhost.

Update: Right now, it is printing out the querystring in the URL and that's it. There will be other updates in the future, stay tuned.

Installation:
Run these commands in the nginx directory:

./configure --with-compat --add-dynamic-module=/usr/local/modules_nginx/nginx-hello-world-module/
make modules
make install

Modify nginx.conf location block:

location = /test {
  hello_world;
}

Run:
nginx

There will be more features to come in the future as I learn more about Nginx and whatnot!
