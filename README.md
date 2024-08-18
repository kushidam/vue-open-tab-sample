# vue-open-tab-sample
Vue.jsを使用して新しいブラウザタブを開き、GETリクエストのパラメータを渡すシンプルなサンプルです。

ユーザーが入力した値をクエリパラメータとしてURLに動的に追加し、新しいタブでサーバーまたは別のリソースにリクエストを送信します。

### 詳細説明

- **`ref`と`v-model`:** `ref`を使って変数をリアクティブにし、`v-model`を使ってユーザーの入力を双方向データバインディングで変数に反映させます。
- **`openNewTab`メソッド:** ユーザーの入力に基づいてクエリパラメータを生成し、新しいタブで指定されたURLを開きます。
- **`encodeURIComponent`:** ユーザーが入力した文字列をエンコードして、URLの一部として使用可能にします。

## 参考資料
- [Vue.js ドキュメント](https://ja.vuejs.org/)
- [MDN Web Docs - URLエンコーディング](https://developer.mozilla.org/ja/docs/Web/JavaScript/Reference/Global_Objects/encodeURIComponent)
- [refとは？](https://qiita.com/yusuke1209kitamura/items/a1a24361b33691dd1818)
- [v-modelについて](https://note.shiftinc.jp/n/n9b4278ce1c9d)
