# TextAlive App API lottie example

Adobe After Effects で作成したアニメーションを Lottie プラグインで書き出したものをビートに合わせて表示するサンプルコードです。 Lottie 関係の部分以外は [basic example](https://github.com/TextAliveJp/textalive-app-basic) そのままです。

リポジトリに含まれている [fw_white.json](src/assets/fw_white.json) が Lottie のアニメーションデータです。他のアニメーションに差し替えて遊んでみてください。アニメーションを作成する環境がない場合は LottieFiles で公開されている無償のアセットを探してみてください。

- デモページ: https://textalivejp.github.io/textalive-app-lottie/
- Lottie: https://airbnb.io/lottie/
- LottieFiles: https://lottiefiles.com/

TextAlive ホストと接続された状態をテストするには [TextAlive App Debugger](https://developer.textalive.jp/app/run/?ta_app_url=https%3A%2F%2Ftextalivejp.github.io%2Ftextalive-app-lottie%2F&ta_song_url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DygY2qObZv24) のページにアクセスしてください。

**English version available in [README.en.md](./README.en.md).**

## 違う楽曲で試すには

TextAlive App API で開発されたWebアプリケーションは、（特定の楽曲向けに作り込んでいない限り）URLのクエリパラメタで `ta_song_url={楽曲のURL}` を指定すると異なる楽曲で演出を試せます。

- [ブレス・ユア・ブレス by 和田たけあき feat. 初音ミク](https://textalivejp.github.io/textalive-app-lottie/?ta_song_url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3Da-Nf3QUFkOU)
- [グリーンライツ・セレナーデ by Omoi feat. 初音ミク](https://textalivejp.github.io/textalive-app-lottie/?ta_song_url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DXSLhsjepelI)

## 開発

[Node.js](https://nodejs.org/) をインストールしている環境で以下のコマンドを実行すると、開発用サーバが起動します。

```sh
npm install
npm run dev
```

## ビルド

以下のコマンドで `docs` 以下にビルド済みファイルが生成されます。 [サンプルコードのデモページ](https://textalivejp.github.io/textalive-app-lottie/) は [GitHub Pages](https://pages.github.com/) で、このリポジトリの `docs` 以下のファイルが提供されています。

```sh
npm run build
```

## TextAlive App API

![TextAlive](https://i.gyazo.com/thumb/1000/5301e6f642d255c5cfff98e049b6d1f3-png.png)

TextAlive App API は、音楽に合わせてタイミングよく歌詞が動くWebアプリケーション（リリックアプリ）を開発できるJavaScript用のライブラリです。

TextAlive App API について詳しくはWebサイト [TextAlive for Developers](https://developer.textalive.jp/) をご覧ください。

---
https://github.com/TextAliveJp/textalive-app-lottie
