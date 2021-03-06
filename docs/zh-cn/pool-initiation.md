## 设置矿池 <!-- {docsify-ignore} -->

!>**以下的教程使用CentOS作为例子，使用Ubuntu或者类似的Linux发行版本请使用正确的命令.**


### 矿池初始化


+ 进入包含Pool可执行文件的文件夹

```console
$ Pool init -p 123
```

>使用-h选项查看帮助文档(如果遇到问题请使用-h查看更多的选项):

```console
$ Pool -h
```

+ 打开Pool的配置文件:

```console
$ vi ~/.pool/conf.json
```

+ 使用以下配置参数修改矿池配置文件:

```
{
        "version": "0.1.0",
        "basip": "198.13.44.159",
        "ethereum": {
                "1": {
                        "id": 1,
                        "apiUrl": "https://mainnet.infura.io/v3/d64d364124684359ace20feae1f9ac20",
                        "paymentService": "0x60eB24514eE5D5Be18685b433E5910C3205D085E",
                        "token": "0x1999ac2b141E6d5c4e27579b30f842078bc620b3"
                },
                "3": {
                        "id": 3,
                        "apiUrl": "https://ropsten.infura.io/v3/d64d364124684359ace20feae1f9ac20",
                        "paymentService": "0x4291d9Ff189D90Ba875E0fc1Da4D602406DD7D6e",
                        "token": "0xAd44c8493dE3FE2B070f33927A315b50Da9a0e25"
                }
        }
}
```

!>**"id": 1为以太坊主网配置，"id": 3为Ropsten测试网络配置**