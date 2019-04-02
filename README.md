# Checklist

Original: https://github.com/snakada/tojimarist

1. 戸締まりチェックリストをブラウザ上で月単位で作成し、最終的には印刷して使います。
2. 戸締まりするチェック項目（玄関、キッチン、火元等）、を自由に追加・削除・ソートができます。
3. 設定したチェック項目は localStorage に保存します。
4. 何ヶ月分でもつくれます。運用としては3ヶ月毎に必要項目を点検しつつ印刷するイメージです。

# example

https://snakada.github.io/tojimarist/

## 主に使ったもの

* [Vue.js](https://jp.vuejs.org/index.html)
* [Vue CLI](https://cli.vuejs.org/)
* [Vuex](https://vuex.vuejs.org/ja/guide/)
* [vue-slicksort](https://www.npmjs.com/package/vue-slicksort)
* [vue-toasted](https://www.npmjs.com/package/vue-toasted)
* [dayjs](https://github.com/iamkun/dayjs)
* [japanese-holidays](https://www.npmjs.com/package/japanese-holidays)
* [Font Awesome](https://fontawesome.com/)
* [Bulma](https://bulma.io/)

## 構成（ざっくり）

```
├── App.vue               // アプリ
├── assets
├── components
│   ├── AddCheckItem.vue  // チェック項目追加フォーム
│   ├── AppHeader.vue     // アプリヘッダ（別になくてもいい）
│   ├── MainSection.vue   // メインセクション（印刷用紙の背景・コンテナ）
│   ├── PrintSheet.vue    // 印刷用紙（成果物、ここに設定がほとんど反映される）
│   ├── SidePanel.vue     // 設定パネル（チェック項目ソート等、いろいろ操作する）
│   └── YearMonths.vue    // 年月操作
├── main.js               // エントリ
└── store.js              // ステート管理
```

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```
