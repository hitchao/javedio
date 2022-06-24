# 常见问题

> 如何添加中字、高清、流出标签
- 在类别或者标签里面输入对应的标签（仅限于：中文、高清、流出），主界面标签戳即可显示


> 如何取消收藏

- 双击第一颗星即可取消


> 如何修改默认视频类型

- 右键【重命名】，修改后，Jvedio 所有视频类型都会相应替换

> 输入网址后无法保存
- 网址仅能保存指定服务器源的网址，如果输入诸如 百度、谷歌之类的网址，测试能通过，但无法保存
- 第一次测试通过后，网址即可保存

> 智能分类没有信息显示
- 请先同步信息，才能智能分类

> 常见网络返回码机器机器原因

| 网络返回码 | 原因                                           |
| ---------- | ---------------------------------------------- |
| 404        | 网址无该资源                                   |
| 403        | 此商品未在您的居住国家公开，需要特定国家的代理 |
| 503, 504   | 网关请求超时，网址可能被屏蔽了                 |
| 302        | 检索过于频繁，服务器源拒绝了请求               |

> 图片无法同步 ？

- 晚上网络不畅
- 进入详情页面，右键-清空信息，然后再同步


> 视频无法导入 ？
- 视频的文件名中必须包含准确的识别码，如 XXX-001 等
- 视频格式仅支持：
3g2,3gp,3gp2,3gpp,amr,amv,asf,avi,bdmv,bik,d2v,divx,drc,dsa,dsm,dss,dsv,evo,f4v,flc,fli,flic,flv,hdmov,ifo,ivf,m1v,m2p,m2t,m2ts,m2v,m4b,m4p,m4v,mkv,mp2v,mp4,mp4v,mpe,mpeg,mpg,mpls,mpv2,mpv4,mov,mts,ogm,ogv,pss,pva,qt,ram,ratdvd,rm,rmm,rmvb,roq,rpm,smil,smk,swf,tp,tpr,ts,vob,vp6,webm,wm,wmp,wmv
- 对于欧美的影片，需要使用欧美扫描与导入，常规扫描无效
- 分段视频的分段规则是否为空，若为空，则填入 `-,_,cd,fhd,-fhd,_fhd`
- 具体问题可查看 `log\Scan` 下当天的 log 文件

> 影片无法成功刮削，图片信息无法下载 ？
- 检查网络是否畅通，网址是否正确输入，Cookie 是否正确输入，并成功测试网络
- 晚上 8:00-12:00 为高峰时间
- 具体问题可查看 `log\Network` 下当天的 log 文件


> Jvedio 支持那些网站 ？

- 网站支持：豆瓣、IMDB


> 为什么缩略图无法显示？

- DB无法同步缩略图，其他的如果有则同步


> 为什么浏览器可以访问网站，而软件无法测试通过 ？
- 检查代理软件是否开启了全局代理


> 如何自己添加图片？

- 对于缩略图/预览图：
将图片复制到SmallPic/BigPic目录下，名字改为识别码且大写，并与软件中显示的识别码完全对应，图片格式仅支持 jpg

- 对于预览图
在 ExtraPic 目录下新建文件夹，名字改为识别码且大写，并与软件中显示的识别码完全对应，该目录放置任何 jpg格式的图片软件都能识别

- 对于演员头像
将图片复制到 Actresses 文件夹中，命名为演员名字，并与软件中显示的演员名字完全对应，仅支持 jpg，比如软件显示 `TonyPark（Tony）`，则图片命名为 `TonyPark（Tony）.jpg`