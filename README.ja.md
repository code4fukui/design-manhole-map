# デザインマンホールマップ

[
![デモを見る](https://img.shields.io/badge/View%20Demo-GitHub%20Pages-2ea44f?style=for-the-badge)
](https://eiichimiyagawa.github.io/design-manhole-map/)

日本全国にあるユニークで芸術的な「デザインマンホール」の蓋を紹介するインタラクティブなウェブマップです。

## デモ

実際のマップはこちらからご覧いただけます:
**[https://eiichimiyagawa.github.io/design-manhole-map/](https://eiichimiyagawa.github.io/design-manhole-map/)**

マーカーをクリックすると、設置場所、写真、デザインの由来など、各マンホールの蓋の詳細情報が表示されます。

## 機能

- **インタラクティブなマップ:** 日本全国をパン・ズームして、デザインマンホールの蓋を探すことができます。
- **詳細なポップアップ:** マーカーをクリックすると、マンホールの名称、住所、座標、詳細な説明を確認できます。
- **高品質な画像:** 各マンホールのユニークなデザインの写真を、マップ上で直接閲覧できます。
- **オープンデータ:** すべての位置データは、シンプルで扱いやすいCSV形式で提供されています。

## 技術スタック

- **[OpenLayers](https://openlayers.org/):** インタラクティブなマップ機能を提供します。
- **[CSV.js](https://github.com/code4fukui/CSV.js):** CSVファイルからのマンホールデータの取得と解析に使用しています。
- **HTML/CSS/JavaScript:** アプリケーション構築に使用しているコアとなるウェブ技術です。

## ローカルでの実行

このプロジェクトをローカルマシンで実行するには、ローカルウェブサーバーを立ち上げてファイルを提供する必要があります。これは、ブラウザのセキュリティポリシー（CORS）により、ローカルファイルの直接読み込みが制限されているためです。

**前提条件:**
- [Node.js](https://nodejs.org/)（`npx`を使用するため）

**手順:**

1.  **リポジトリのクローン:**
    ```sh
    git clone https://github.com/eiichimiyagawa/design-manhole-map.git
    cd design-manhole-map
    ```

2.  **ローカルサーバーの起動:**
    `npx`を使用して`http-server`パッケージを実行するのが簡単な方法です。
    ```sh
    npx http-server
    ```

3.  **ブラウザで開く:**
    サーバーによって提供されたURL（例: `http://127.0.0.1:8080`）にアクセスします。

## データソース

マンホールの蓋のデータはCSVファイルとして利用可能であり、下水道広報プラットフォームから取得したものです。

- **オープンデータCSV:** [design-manhole-map/data.csv](https://eiichimiyagawa.github.io/design-manhole-map/data.csv)
- **情報元:** [マンホールカード検索 | 下水道広報プラットフォーム](https://www.gk-p.jp/mhcard/?pref=18#mhcard_result)

## ライセンス

MIT License — 詳細は [LICENSE](LICENSE) を参照してください。
