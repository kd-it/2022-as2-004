# 問題4

ストレージクラス standard を用いたダイナミックプロビジョニングを利用するPVC `contents` をマウントするapache2のポッドを作成せよ。
ファイルはex4.ymlを使うこと。

- pvc/contentsの仕様
    - ストレージクラスstandard(省略可能)を使ってダイナミックプロビジョニングとする
    - ストレージ容量は128Mi(以上)を要求すること
    - アクセスモードはReadWriteOnceとしておく
- pod/ex4の仕様
    - イメージ httpd を用いること
    - pvc/contentsを/usr/local/apache2/htdocsにマウントすること
    - ポートは80番を使う旨を宣言しておくこと

ファイルex4.ymlを適用することで、ストレージ・ワークロード(ポッド)を生成するようにすること。

```
PS> kubectl apply -f ex4
persistentvolumeclaim/content created
pod/ex4 created
```
