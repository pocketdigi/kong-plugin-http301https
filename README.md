Kong plugin http301https
====================

A simple kong plugin that 301 redirect http request to https version, for example:

if your user visit your site with http:

```
http://www.example.com/xxx.php?a=b
```

this plugin will redirect to:

```
https://www.example.com/xxx.php?a=b
```

### How to use

1. clone the code:

    ```
    git clone git@github.com:pocketdigi/kong-plugin-http301https.git
    ```

2. install 

    ```
    cd kong-plugin-http301https
    luarocks make
    ```
3. Edit /etc/kong/kong.conf, uncomment`plugins = bundled` add http301https

    ```
    plugins = bundled,http301https
    ```
4. Restart kong

5. Add plugin to your service


