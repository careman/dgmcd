title: 东莞谢岗福易门业
---
谢岗福易门业是谢岗不锈钢品牌门窗产品综合服务商,集室内门窗装饰设计、门窗产品定制、门窗安装服务于一身,提供一揽子装修装饰安防产品解决方案。

## 联系方式


``` 
电话：13717323108 陈生老表
地址：东莞市谢岗镇花园大道236号
```

## 主营产品

产品类别 | 产品介绍 | 适用范围
--- | --- | ---
`不锈钢门` | Enable debug mode. Display debug messages in the terminal and save `debug.log` in the root directory. | `false`
`实木门` | Enable safe mode. Don't load any plugins. | `false`
`铝合金门` | Enable silent mode. Don't display any messages in the terminal. | `false`
`防护栏杆及楼梯扶手` | Specify the path of the configuration file. | `_config.yml`
`防护网及窗花` | Specify the path of the configuration file. | `_config.yml`

## Load Files

Hexo provides two methods for loading files: `load` and `watch`. `load` is used for loading all files in the `source` folder as well as the theme data. `watch` does the same things `load` does, but will also start watching for file changes continuously.

Both methods will load the list of files and pass them to the corresponding processors. After all files have been processed, they will call upon the generators to create the routes.

``` js
hexo.load().then(function(){
  // ...
});

hexo.watch().then(function(){
  // You can call hexo.unwatch() later to stop watching.
});
```

## Execute Commands

Any console command can be called explicitly using the `call` method on the Hexo instance. Such a call takes two arguments: the name of the console command, and an options argument. Different options are available for the different console commands.

``` js
hexo.call('generate', {}).then(function(){
  // ...
});
```

## Exit

You should call the `exit` method upon successful or unsuccessful completion of a console command. This allows Hexo to exit gracefully and finish up important things such as saving the database.

``` js
hexo.call('generate').then(function(){
  return hexo.exit();
}).catch(function(err){
  return hexo.exit(err);
});
```
