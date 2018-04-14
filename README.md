nginx.repo API
====

CentOSとかでいちいち`nginx.repo`の記述を探してvi立ち上げて入力するのがめんどくさい。そんなあなたに。

## Description

nginx公式にに沿った`nginx.repo`を返すだけのページ。

https://www.nginx.com/

## Usage

curlで引っ張ってきて帰ってきたやつをyumリポジトリに追加してあげる。

CentOS
```
$ sudo curl https://yoshiken.github.io/nginx.repo-api/centos.html > /etc/yum.repos.d/nginx.repo
```

RHEL
```
$ sudo curl https://yoshiken.github.io/nginx.repo-api/rhel.html > etc/yum.repos.d/nginx.repo
```

あとは`sudo yum install nginx`すればオワリ。

RHELは持ってないので実際これで合ってんのかしらん。
