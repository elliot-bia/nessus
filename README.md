# nessus docker 破解版
[English version](README-en.md)


此项目仅供非营利性学习研究，请勿用作非法用途，如有侵权请及时联系删除


[more info](https://twitter.com/Elliot58616851)

# 用法/Usage
`docker run -itd --name=ramisec_nessus -p 8834:8834 ramisec/nessus`  (只有 497MB !!!)  
就是这么简单! 但是需要下面一行代码更新插件🤣


# 更新
`docker exec -it ramisec_nessus /bin/bash /nessus/update.sh`

__提醒__  
如果你无法更新成功，请检查网络连接  

# 账号密码
account：admin  
password： 每个版本密码就是一个彩蛋！ Easter egg！CHECK the Change Version   
让大家探索一下，避免伸手党，如果解出了密码，自己用就好，不要公开哟😉  

# 说明/Readme
这个破解原本是自用的，也没打算公开出来    
但是昨天在使用fahai破解版awvs的时候，看到了这么一句话：  
`Thank's fahai && Open Source Enthusiast `  
 <img src="https://user-images.githubusercontent.com/40572216/174698816-440d4969-f9d6-4c7d-982c-9af9c4a3e875.png" width = "400" height = "200" alt="图片名称" align=center />
 
于是我就在思考，我用了那么多开源项目，那我又做出了多少贡献？    
索性将此项目公开，也算为网安做一点贡献    
如果没有意外，会持续更新，毕竟我也要用    
~~就不把自动更新插件版本弄出来了，先用着吧！~~  
已更新！（20220722）


# 更新日志

## v3 20220722
__重磅更新：自动更新插件docker版的Nessus搞出来了！__

用法： `docker run -itd --name=ramisec_nessus -p 8834:8834 ramisec/nessus`  
下载下来的容器是没有更新插件的  
之后再更新插件，更新插件的命令都相同：   
`docker exec -it ramisec_nessus /bin/bash /nessus/update.sh`  
下次要更新的话，执行相同的命令即可


## v2 20220621
更新20220620最新版插件，同时采用2个版本 nessus/nessuslite  
前者是已经破解好并且编译好插件，开箱即用    
后者开机后需要等待几分钟编译插件    
password:   
`U2FsdGVkX19WZv+QOe8awVyJwXDPSNSIC1X4AMNA4+3rO8mL/3HZ+mS/Or3DhcWXKs0WHfvOH1q/YNtVdXnaHg==`  
__tips__: github/elliot-bia  


> ~~# 旧版用法/Usage~~
> ~~`docker run -itd -p 8834:8834 ramisec/nessus`   (4.73GB)~~
> ~~或者/or~~  
> ~~`docker run -itd -p 8834:8834 ramisec/nessuslite` (3.55GB)~~  
> ~~前者不需要编译，适合低性能高带宽机器~~
> ~~后者需要编译，适合高性能低带宽机器~~
> ~~The former does not require compilation and is suitable for low-performance high-bandwidth machines~~  
> ~~The latter requires compilation and is suitable for high-performance low-bandwidth machines~~  
> ~~What? high-performance and high-bandwidth machines? Never mind, just use it! have fun!~~


其实除了以上解密，还有另一种很简单的办法，让大家挖掘😆


