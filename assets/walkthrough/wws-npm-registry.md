Run the following command on a terminal/console window to set the registry [https://npm.worldwidestreams.io](https://npm.worldwidestreams.io) for `@xstream` and `@wws_public` packages. This alternative registry is needed because these packages are not published on the [official]( https://registry.npmjs.org) npm registry. Use the credentials provided (check your email) for the prompted `user` and `password`.
```bash
npm login --registry=https://npm.worldwidestreams.io
```
After logged into https://npm.worldwidestreams.io, set the scope registry for `@xstream` and `@wws_public`.
```bash
npm config set @xstream:registry  https://npm.worldwidestreams.io/
npm config set @wws_public:registry  https://npm.worldwidestreams.io/
```
You can check the current npm configuration by running the following command:
```bash
npm config list
```
The output should include these two entries:

``` 
@wws_public:registry = "https://npm.worldwidestreams.io/" 
@xstream:registry = "https://npm.worldwidestreams.io/" 
```
If you encounter a connection timeout while logging in and you are connected to the NOKIA network,
run the following commands to properly configure the NOKIA proxy:
```bash 
npm config set proxy http://proxy-server-url:port
npm config set https-proxy http://proxy-server-url:port
```
Use the nearest proxy to your location e.g., `http://135.245.192.7:8000`



