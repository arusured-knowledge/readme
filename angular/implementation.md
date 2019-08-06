# 実装編

- [ngForでテーブルっぽく](##ngForでテーブルっぽく)
- [serviceでのデータ持ち方(非同期で扱いやすく)](serviceでのデータ持ち方(非同期で扱いやすく))
- [angular material](##angular&nbsp;material)
- [flex layout](##flex&nbsp;layout)
- [routing](##routing)
- [pipe](##pipe)
- [pager](##pager)
- [reactive form](##reactive&nbsp;form)
- [scss](##scss)

## ngForでlist表示
list表示した時の例です。<br>
cssを駆使すれば、テーブルっぽくできるはずです。<br>
[サンプル](./../../angular-list-table)

ちなみに、jsonデータを気軽に使いたい時は、`tsconfig.json`に

```tsconfig.json
{
    "compilerOptions": {
        "resolveJsonModule": true,
        "esModuleInterop": true
    }
}
```
を追記すると良い。

### 参考
- [Angular公式ページ](https://angular.jp/tutorial/toh-pt2)
- [【Angular7】 json を module として扱う](https://qiita.com/MasanobuAkiba/items/98a678430fa192c0f8c5)

## serviceでのデータ持ち方(非同期で扱いやすく)
## angular material
## flex layout
## routing
## pipe
## pager
## reactive form
## scss