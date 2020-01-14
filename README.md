#使用python3 编写

##使用方式

###python ssr_ss_decode.py

###在提示的信息里面输入令你难受的ssr或者ss，就可以直接解析了


##梳理下ss和ssr

###ss链接：在 base64 编码之前，ss链接的格式如下

>ss://method:password@server:port
>
>我们看到的都是进行过base64编码的数据及ss://base64编码
>
>所以ss链接可以直接使用base64 进行解码就可以完成解析
>
###ssr链接：在base64编码前，ssr格式如下：

>ssr://server:port:protocol:method:obfs:password_base64/?params_base64
>
>password_base64和params_base64分别是password和params被base64编码后的字段
>所以需要进行对此base64解码