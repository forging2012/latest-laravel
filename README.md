Latest-laravel
==============

每天更新的 Laravel 完整包，下载直接可以运行（已经 `composer install` 了，也就是已经有了vendor目录）。 [赞助本项目](#%E8%B5%9E%E5%8A%A9dollar)

- 主要解决的问题：

    - 不会用 `composer` 或者不太会用；
    - `composer` 装不上或者装上了但是 `composer install` 特别慢。

- 更新频率：
    > 每天上午 :clock830:`8:30`

- Laravel 分支
    - `master` 也就是目前的5.*, 对应包名： `laravel-master.tar.gz`
    - `develop` 开发版，对应包名：`laravel-develop.tar.gz`

 如果你发现目录中不存在某个包，那么这个包就是打包失败，很有可能是开发版作者的修改还未完成以至于打包失败。错误日志见[issue](https://github.com/overtrue/latest-laravel/issues)

# 使用
1. 下载本项目里的 `laravel-xxxxx.tar.gz` 文件, 然后在你的 www 目录下触压；
2. 给 `storage` 目录的写权限，*unix 用户参考：`chmod -R 755 ./storage`；

完成，访问 `http://localhost/laravel/public/` 即可看到欢迎页面。

_本项目打包时会清除首页模板的 Google 字体引用，避免半天打不开首页的情况。_

## 原理

:bulb: 从 `laravel/laravel` 更新 :inbox_tray: :arrow_right:  使用 `composer install` 安装依赖 :arrow_right: 打包:package: :arrow_right:  push 到 GitHub :outbox_tray:

更多请直接参考脚本：[update.sh](https://github.com/overtrue/latest-laravel/blob/master/scripts/update.sh) :sweat_smile: shell 功底差，请多指教！

## 说明
- 本项目的前提你还是要满足基本条件才能正常运行 Laravel：`php >= 5.4 && mcrypt 拓展`
- `public` 目录才是网站根目录，所以如果你要添加虚拟主机请把 `document root` 设置到 `public`，至于为什么这里不想做过多的解释，你就这么认为就好了。

## <del>赞助:dollar:</del>
<del>本项目运行在crissic机器上，如果您觉得对你有帮助愿意捐助的话有两种方式：

1. 我的支付宝：anzhengchao@gmail.com
2. 直接转到我的PayPal：anzhengchao@gmail.com（有PayPal的朋友推荐使用此方式，免去我找淘宝充PayPal的麻烦:sweat_smile:）

请留下您的联系方式，感谢！</del>

感谢以下朋友的赞助：

<table>
<tr><th>名称</th><th>金额</th><tr>
<tr><td> Laravel中文网创始人 王赛<a href="https://github.com/wangsai">@wangsai</a></td><td>￥100</td>
</table>

## 关于Laravel
请参考：http://laravel.com/ 或者 中文版:http://www.golaravel.com/

