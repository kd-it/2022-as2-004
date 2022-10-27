# 問題2: 問題1を使うPVCを作成せよ

問題1で作成したpv/ex1を要求するpvc/ex1を作成せよ。
記述はこのディレクトリにあるex2.ymlに記述すること。

こちらもマニフェスト適用後にpvcの状態をチェックすることでBound状態になっているかで確認できます。

```
PS> kubectl get pvc
NAME          STATUS   VOLUME   CAPACITY   ACCESS MODES   STORAGECLASS   AGE
ex2           Bound    ex1      128Mi      RWO            local          2s
```
