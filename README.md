# About

Hexo 主题 [Clarity](https://github.com/guozhenyi/hexo-theme-clarity) 的第三方库。

## 自托管使用

如果 CDN 失效，可以把这些文件传到项目 `assets/lib` 目录下，然后把 `https://unpkg.com` 替换为 `/assets/lib` 。

## CDN 自部署方法

不管是 unpkg 还是 jsdelivr，在国内速度都比较慢，还可能被 Qiang。

最简单的方法就是搞 jsdelivr 反向代理。

这里我用的是个笨办法，把 Clarity 主题所用到的第三方库，从 npm 下载下来，解压，按 CDN 上的资源路径，整理成一致的目录结构。

然后把所有第三方库，上传到云存储中，再通过 CDN 去访问，这样就实现了类似 jsdelivr 反代的效果。

### 1. 多吉云 CDN






