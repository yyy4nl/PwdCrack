# 工具介绍

最近遇到的若依和Jeecg比较多，有的站通过其他方式拿到数据库权限之后，数据库中的web用户的密码是加密的，无法获取管理员或者其他用户的明文密码，尝试过用cmd5进行解密，但是没有结果。此工具就是为了解决这个问题写的，如有问题还请多指教。

比如下面这个从若依二开数据库中翻到的密码，明文密码就是123456。

![](E:\圈子\PwdCrack_tool\PwdCrack\img\cmd5.png)

密码是123456，但是cmd5没有匹配到，加入后台进行破解的话还会扣两块，但是使用这个工具就可以爆破出来

![](E:\圈子\PwdCrack_tool\PwdCrack\img\jiemi.png)

同样的jeecg的密码，cmd5也没有匹配到，但是使用工具可以匹配到

![](E:\圈子\PwdCrack_tool\PwdCrack\img\cmd52.png)

![](E:\圈子\PwdCrack_tool\PwdCrack\img\jiemi1.png)

![](E:\圈子\PwdCrack_tool\PwdCrack\img\jiemimi.png)

### ruoyi密码破解

选择密码字典之后，在密文输入框中输入数据库中找到的加密密码，点击开始爆破之后会自动爆破（线程数为CPU核心数减一），爆破完成之后会在jar包所在目录生成ruoyi_result.txt文件，文件中保存了破解成功的密码。

![](E:\圈子\PwdCrack_tool\PwdCrack\img\ruoyi.png)

![](E:\圈子\PwdCrack_tool\PwdCrack\img\ruoyi_result.png)

### Jeecg密码破解

同理选择密码字典后可直接开始爆破

![](E:\圈子\PwdCrack_tool\PwdCrack\img\jeecg.png)

![](E:\圈子\PwdCrack_tool\PwdCrack\img\jeecg_result.png)