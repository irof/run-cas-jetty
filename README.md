ローカルでCASをとりあえず動かすやつ
========================================

## 使ってるもの

* cas-server-webapp:4.0.1
* jetty-maven-plugin:8.1.1.v20120215

## 使い方

* `mvn jetty:run-war` と叩く。
* https://localhost:9443/ を見る。

## 鍵さん

https を使うために実行時に keytool-maven-plugin:generateKeyPair を叩いてます。
ついでに exportCertificate も叩いてるので、 LocalCAS.crt が直下に吐かれる。必要に応じて。

## メモ

jetty9にしようと思ったらなんか設定のしかた変わってるっぽかったのでこれから。。。

