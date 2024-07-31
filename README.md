# Cloudflare_VLESS

在 CloudFlare Workers 或 Pages 部署 VLESS 节点

## 部署教程

部署教程自行前往YouTube搜索

进入Cloudflare官网

进入Workers & Pages，创建一个新Worker或Pages

进入代码后台，把原来的js全部删掉，复制本项目_worker.js中的所有代码，粘贴进js里

用V2RayN生成一个UUID，替换第八行的UUID，保存


访问 https://DOMAIN.workers.dev/UUID ，即可查看节点明文配置信息

访问 https://DOMAIN.workers.dev/UUID/base64 ，即可使用 Base64 通用客户端订阅

访问 https://DOMAIN.workers.dev/UUID/clash ，即可使用 Clash 节点订阅

访问 https://DOMAIN.workers.dev/UUID/sb ，即可使用 Sing-box 节点订阅

将节点订阅导入V2RayN或V2RayNG，即可使用，或搭配Cloudflare的IP优选使用，替换原本的地址（其他的不要动）

默认域名为 www.visa.com.hk ，可以替换成任意套了Cloudflare CDN的域名（如www.gov.se speed.cloudflare.com leslieblog.top），也可以搭配IP优选将地址改为Cloudflare EndPoint 边缘IP

## 鸣谢

项目大部分代码来自 https://github.com/Misaka-blog/cf-wkrs-pages-vless/tree/main ，原作者停更，克隆此仓库更新

鸣谢项目
zizifn：https://github.com/zizifn/edgetunnel
3Kmfi6HP：https://github.com/3Kmfi6HP/EDtunnel
cmliu：https://github.com/cmliu/edgetunnel

