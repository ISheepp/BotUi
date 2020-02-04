既然是JavaScript，那么支持HTML是肯定的（废话），也适用于WordPress,Typecho等主题（还是废话）。

HTML插入到</body>标签前。

WP等：在主题footer.php文件</body>标签前上一行输入以下代码

```
<script type="text/javascript">//樱花
 var system ={}; 
 var p = navigator.platform; 
 system.win = p.indexOf("Win") == 0; 
 system.mac = p.indexOf("Mac") == 0; 
 system.x11 = (p == "X11") || (p.indexOf("Linux") == 0); 
 if(system.win||system.mac||system.xll){//如果是电脑
 
 $.getScript("https://cdn.jsdelivr.net/gh/ivampiresp/special-JavaScript/yinghua.js");
 }else{ //如果是手机
 
 }
 </script>
```

保存后，刷新缓存（如果有），然后看看效果吧。