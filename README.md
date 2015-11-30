pickles2/broccoli-module-bootstrap3
=========

Bootstrap3 modules for [Pickles 2](http://pickles2.pxt.jp/) and broccoli-html-editor.



## 導入方法 - Setup

### 1. [Pickles 2](http://pickles2.pxt.jp/) をセットアップ

### 2. composer.json に、パッケージ情報を追加

```
{
    "require": {
        "pickles2/broccoli-module-bootstrap3": "dev-master"
    }
}
```

### 3. composer update

更新したパッケージ情報を反映します。

```
$ composer update
```

### 4. config.php を更新

モジュール設定を書き加えます。

```
<?php
return call_user_func( function(){

	/* (中略) */

	@$conf->plugins->px2dt->paths_module_template["Bootstrap3"] = "./vendor/pickles2/broccoli-module-bootstrap3/modules/";

	/* (中略) */

	return $conf;
} );
```

## License

MIT License


## Author

- (C)Tomoya Koyanagi <tomk79@gmail.com>
- website: <http://www.pxt.jp/>
- Twitter: @tomk79 <http://twitter.com/tomk79/>
