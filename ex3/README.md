# 問題3

問題1,2を結合して1つのファイルで両方を適用できるマニフェストex3.ymlを作成せよ

ヒント: マニフェストは "---" を挿入することで論理的に別のものを記入可能です。

これにより、以下の操作でまとめて適用できるようになります。

```
PS> kubectl apply -f ex3.yml
persistentvolume/ex1 created
persistentvolumeclaim/ex2 created
```
