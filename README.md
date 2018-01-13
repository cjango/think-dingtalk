# think-dingtalk
===============

[![Latest Stable Version](https://poser.pugx.org/cjango/think-dingtalk/version)](https://packagist.org/packages/cjango/think-dingtalk)
[![Total Downloads](https://poser.pugx.org/cjango/think-dingtalk/downloads)](https://packagist.org/packages/cjango/think-dingtalk)
[![Latest Unstable Version](https://poser.pugx.org/cjango/think-dingtalk/v/unstable)](//packagist.org/packages/cjango/think-dingtalk)
[![License](https://poser.pugx.org/cjango/think-dingtalk/license)](https://packagist.org/packages/cjango/think-dingtalk)

#### 钉钉SDK For thinkphp5

> 该项目依赖于thinkphp5.0.*

## 安装
> composer require cjango/think-dingtalk

## 配置
> 配置文件位于 `application/extra/dingtalk.php`

```
return [

];
```

## 使用方法
```
// 引用命名空间
use cjango\dingtalk\Dingtalk;

// 获取全部关注用户
Dingtalk::get('user')->all();

// 网页用户直接跳转授权
Dingtalk::get('oauth')->url($callback);

// 回调页面中直接调用
Dingtalk::get('oauth')->token();

// 获取错误信息
Dingtalk::error()
```
