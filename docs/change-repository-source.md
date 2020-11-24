## 更换各种软件源

[回到首页](./index.md)

因为各种不可控的原因，在更新和下载某些软件的时候因为连不上服务器导致更新失败，不仅极大的影响工作，而且影响心情。更换成国内的加速镜像源可以部分解决问题，考虑到不同的镜像源的同步策略和实际的情况，可能会有一定程度的延迟，不能像官方源那样及时。

### 更换debian/ubuntu的apt软件源

编辑`/etc/apt/sources.list`文件，修改其中的地址为镜像地址，比如中科大的`mirrors.ustc.edu.cn`或者上海交大的`mirrors.sjtug,sjtu,edu,cn`等等，保存后执行`sudo apt update`更新缓存

### 更换Homebrew源

Homebrew拉取Github的文件，而Github的连接速度很不稳定，而且很慢。更换方法可以参考[这里](https://frankindev.com/2020/05/15/replace-homebrew-source/)，或者按照镜像源官方的方法。

### 更换树莓派镜像源

如果是安装的是官方系统`Raspbian`，那么更换方法和Debian几乎一样，修改`/etc/apt/sources.list`和`/etc/apt/sources.list.d/raspi.list`文件。