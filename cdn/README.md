# CDN


## PUSH OR PULL?

+ PUSH CDN
  + ***特点***
    + `内容`经常发生变化
    + 需要开发针对 CDN 的推送服务接口
    + 提前推送`内容`到 CDN 上，节省站点带宽资源
    + 提前推送`内容`到 CDN 上，防止流量高峰占满站点带宽资源，同时靠近用户提供就近资源访问，服务体验更好
  + ***适用场景***
      + 站点包含视频、音频等内容，或提供文件下载等服务


+ PULL CDN
  + ***特点***
    + 上手简单，易配置
    + `内容`不经常发生变化，可以长期（比如 24 小时）缓存在 CDN 上
    + 不能自由的控制`内容`缓存的过期时长
    + 由于第一次请求会转发到服务器上，所以， 系统、服务器等最好做好充分的优化。不过，即便如此，第一次请求仍然耗时会比较多长
  + ***适用场景***
    + 高流量、低下载的站点（PULL 的方式让最热的`内容`缓存在 CDN 中）

