## Miner Configuration <!-- {docsify-ignore} -->

!>**This steps are for CentOS if you install Pool in Ubuntu please use the console command accordingly.**


### Initiation <!-- {docsify-ignore} -->

+ Entering the folder that contain the HOP file

```console
$ HOP init -p 321
```

>Check the help command to see more option(Please use -h option in any steps to check more options):

```console
$ HOP -h
```

+ Open Miner settings:

```console
$ vi ~/.hop/conf.hop
```

+ Change the settings as following:

```
{
        "BAS": "198.13.44.159",
        "id": 3,
        "apiUrl": "https://ropsten.infura.io/v3/fe5ffffba0bf46bb9dc27fd5e04cd6cb",
        "paymentService": "0x4291d9Ff189D90Ba875E0fc1Da4D602406DD7D6e",
        "token": "0xAd44c8493dE3FE2B070f33927A315b50Da9a0e25"
}
```