# 実装編

- [ngForでlist表示](#ngForでlist表示)
- [serviceでのデータ持ち方(非同期で扱いやすく)](#serviceでのデータ持ち方非同期で扱いやすく)
- [angular material](#angular-material)
- [flex layout](#flex-layout)
- [routing](#routing)
- [pipe](#pipe)
- [pager](#pager)
- [reactive form](#reactive-form)
- [scss](#scss)

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
TODO serviceがsubject型の配列を持ち、初回呼び出しでobservable部分を呼び出し元に渡す。<br>
そして、subscribeしている例を作る。

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
TODO flex layoutのインストール方法と、ちょっとしたサンプルを作ってみる。

## routing
TODO 普通にroutingしているバージョンと、lazyloadしているバージョンのサンプルを作ってみる。

## pipe
TODO 既に用意されているpipeを使ったものと、自作pipeを使ったもののサンプルを作ってみる。

## pager
レコードが複数あるが、表示したい領域に収まらない。そんな時に使う機能です。<br>
Angular materialには便利な[pager](https://material.angular.io/components/paginator/overview)が用意されていますが、table向けとのこと。<br>
ngForでリスト表示することもあるので、何とか使えないかチャレンジしたのが[こちら]()

## reactive form
TODO reactive formのサンプルを作ってみる。formBuilderを使うパターンとformGroupをnewするパターン。<br>
出来たら、必須入力やバリデーションの部分も作ってみる。

## scss
TODO なんか便利そうな事があったら、ここにメモする。

