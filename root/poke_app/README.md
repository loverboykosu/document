# はじめに

React の学習を兼ねて、ポケモン図鑑アプリを作成しました。今回は、デプロイまで行っています！手順を説明するものではなく、あくまで、実施したことの備忘録がわりです。

# 全体概要

はじめに、ポケモン図鑑アプリの UI は以下のようになっています。

| ![sample1.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/693671/8edd1979-177c-4c41-b90e-9f455492edda.png) |
| :-------------------------------------------------------------------------------------------------------------------------: |

構成はシンプルで、以下の 3 つの要素から構成されています。

- ポケモン図鑑
- 検索
- ページ

以下が今回のシステムの概要です。
|![sample2.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/693671/aad7a8dc-cd9b-4d3d-a253-a20c644e24c1.png)|
|:-:|

# フォルダ構成

src 以下のフォルダ構成は以下のようになっています。

```
├── App.css
├── App.jsx
├── assets
│   └── react.svg
├── components
│   ├── Page.jsx
│   ├── Poke.jsx
│   └── Search.jsx
├── index.css
├── lib
│   └── poke.jsx
└── main.jsx
```

components フォルダに実際の UI などが記載されています。
また、lib フォルダには poke_api からデータを取得する処理が記載されています。

# render にデプロイ

reder というサービスにデプロイするには以下の手順を踏む必要があります。

- アカウントの作成
- github と連携
- build
- デプロイ

無料モードもあるので、ぜひ試してみてください！

[ポケモン図鑑アプリ URL](https://poke-app-dqdj.onrender.com/)

以下にソースコードの github リンクを置いておきます。
https://github.com/loverboykosu/poke_app
