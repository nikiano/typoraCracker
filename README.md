# typora Cracker
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FMas0nShi%2FtyporaCracker.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FMas0nShi%2FtyporaCracker?ref=badge_shield)


A patch and keygen tools for typora.

中文说明请戳[这里](README_CN.md)

## WARNING
```
FOR STUDY AND DISCUSSION ONLY, PLEASE DO NOT ENGAGE IN ANY ILLEGAL ACTS.
ANY PROBLEMS ARISING FROM THIS WILL BE BORNE BY THE USER (YOU).
```

## Features

- Supports ALL OS supported by typora

## Usage

1. `pip install -r requirements.txt`
2. `python typroa.py --help`
3. read and use.
4. patch License.js.
5. replace app.asar.
6. run keygen.
7. enjoy it.


## Example

```shell
> python typroa.py --help
usage: typora.py [-h] [-u] [-f] asarPath dirPath

[extract and decryption / pack and encryption] app.asar file from [Typora].

positional arguments:
  asarPath    app.asar file path/dir [input/ouput]
  dirPath     as tmp and out directory.

optional arguments:
  -h, --help  show this help message and exit
  -u          pack & encryption (default: extract & decryption)
  -f          enabled prettify/compress (default: disabled)

If you have any questions, please contact [ MasonShi@88.com ]

> python typora.py {installRoot}/Typora/resources/app.asar workstation/outfile/
⋯
> python typora.py -u workstation/outfile/ workstation/outappasar
⋯
> cp {installRoot}/Typora/resources/app.asar {installRoot}/Typora/resources/app.asar.bak
> mv workstation/outappasar/app.asar {installRoot}/Typora/resources/app.asar
# (patch code)
> node keygen.js
XXXXXX-XXXXXX-XXXXXX-XXXXXX
> typora
# (input info)
email: crack@example.com
serial: XXXXXX-XXXXXX-XXXXXX-XXXXXX
```

## LICENSE
 MIT LICENSE

[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FMas0nShi%2FtyporaCracker.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FMas0nShi%2FtyporaCracker?ref=badge_large)


# 使用
这个Cracker可以用来生成钥匙，也可以，修改旧版本的到期问题。目前只试过用来修改到期问题，
所以只简单记录下修改版本到期时间这个的步骤。

## 使用流程
1. 把文件，project，项目（whatever）下载（clone）下来，找个地方放，姑且把这个地址叫：c:\Typora_Cracker\
2. 看看你Typora的地址： c:\Typora
3. 安装python
4. 打开cmd， 
  ```shell
  cd \d c:\Typora_Cracker\
  pip install -r requirements.txt
  python typora.py c:\Typora\resourse\app.asar . 
  # 中间步骤 打开 dec_app\Liense.js 这个文件，替换 1636297098336 为 4713176400336 （总共有四处）文件在Typora_Cracker里面 
  # 修改 dec_app 为 app
  python typora.py -u app\ .
  # 复制 app.asar 文件，替换掉 typora\resourse\app.asar 
  ```
  
