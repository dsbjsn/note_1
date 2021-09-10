# 解决Android P系统限制了明文流量的网络请求，P之下的版本没有影响
```
<?xml version="1.0" encoding="utf-8"?>
<!--解决Android P系统限制了明文流量的网络请求，之下的版本没有影响，所以okhttp3会抛出该异常-->
<!--添加目录：res/xml/network_security_config-->
<!--Manifest文件->application 添加android:networkSecurityConfig="@xml/network_security_config" -->
<network-security-config>
    <base-config cleartextTrafficPermitted="true" />
</network-security-config>  
```
