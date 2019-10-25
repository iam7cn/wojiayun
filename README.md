# wojiayun
粒子云我家云防止掉盘补丁
``` bash
curl http://www.wdmomo.fun:81/script/liziyun/loss
```
![福祖保佑](http://bbs.nas66.com/data/attachment/forum/201910/09/112854elo0glqwok88yykk.png)
<p>我家云&粒子云&掉盘云-终极软件不掉盘

<p>系统：[Liziyun-Armbian-OMV-EntWare.img]
> 终端默认账号：`root` 密码：`wdmomo` | `WEB`端默认账号：`admin` 密码：`wdmomo`| 其他看`web`端注释说明
> `WEB`端登录：默认盒子`IP`，备注集成的aira2，transmission以及百度云`web`端的注释说明有误默认下载地址为：`/sharedfolders/downloads`
> 如内存不够可关闭2个swap释放内存

``` bash
swapoff /dev/zram4
swapoff /dev/zram3
echo 3 > /proc/sys/vm/drop_caches
```
  
<p>群内最新测试可防止掉盘，感谢群友`ride_wind`测试，感谢恩山大神提供文件，简化操作制作一键修复补丁
需联网在ssh下运行，仅测试`Liziyun-Armbian-OMV-EntWare.img`，其他系统自行测试
  
``` bash
wget -O - http://www.wdmomo.fun:81/script/liziyun/update.sh | /bin/sh
```
 或者如下命令
  
``` bash
wget -q http://www.wdmomo.fun:81/script/liziyun/update && chmod u+x update && ./update
```
