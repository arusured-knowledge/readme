# 実装編

- [ngForでlist表示](##ngForでlist表示)
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
[サンプル](https://github.com/arusured-knowledge/angular-list-table)

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
モジュールを利用することで、モダンなデザインをお手軽に適用できるもの。<br>
Googleが作成している。<br>
[公式ページ](https://material.angular.io/)を元に、インストールをしていく。

1. npmでインストールする。

    ```shell
    npm install --save @angular/material @angular/cdk @angular/animations
    ```

2. 使用したいモジュールで「BrowserAnimationsModule」か「NoopAnimationsModule」をimportする。

3. angular materialの使いたい機能を、使用したいコンポーネントでimportする。

4. `styless.css`にテーマをimportする。

5. ジェスチャー系の機能を使うために、「hammerjs」をnpmでインストールする。

6. material iconsを使うために、`index.html`にリンクを追記する。



## flex layout
## routing
## pipe
## pager
レコードが複数あるが、表示したい領域に収まらない。そんな時に使う機能です。<br>
Angular materialには便利な[pager](https://material.angular.io/components/paginator/overview)が用意されていますが、table向けとのこと。<br>
ngForでリスト表示することもあるので、何とか使えないかチャレンジしたのが[こちら]()

## reactive form
## scss