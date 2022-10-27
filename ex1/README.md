# 問題1

以下のPVを作成せよ

- PV名 ex1
- 容量 128Mi(128MB)
- アクセスモード ReadWriteOnce
- ストレージクラス local
- hostPath方式で、/tmp/ex1 ディレクトリを使用する

生成できているかは、 `kubectl get pv` で確認できる。

```
PS> kubectl get pv
NAME   CAPACITY   ACCESS MODES   RECLAIM POLICY   STATUS      CLAIM   STORAGECLASS   REASON   AGE
ex1    128Mi      RWO            Recycle          Available           local                   7s
```

添付しているマニフェストex1.ymlに記述すること。
