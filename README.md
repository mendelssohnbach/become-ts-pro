# become-ts-pro

Learn from the book "Introduction to TypeScript for Professionals"

# このレポジトリについて

購入した書籍を写経しています。

## 書籍について

次の書籍を用いて **TypeScript** の学習を行う

[プロを目指す人のための TypeScript 入門](https://gihyo.jp/book/2022/978-4-297-12747-3)
[正誤表](https://gihyo.jp/book/2022/978-4-297-12747-3/support)
[サンプルコード](https://gihyo.jp/assets/files/book/2022/978-4-297-12747-3/download/ProTypeScript_SampleCode.zip)

## 書籍の環境

- Node.js v16.8.0
- TypeScript 4.6.2
- @types/node 14.14.10

## コラム

- コラム 1: `tsconfig.json` で独自機能を制限することはできない
  - `enum`: **ユニオン型** に置き換える
  - `namespace`: **ES Modules** に置き換える

```TypeScript
// enum の代わりに
export const Status = {
    Active: "ACTIVE",
    Inactive: "INACTIVE",
} as const;

export type Status = typeof Status[keyof typeof Status];
```

**ESLint** でルールとして制限する

## プログラムの実行

```Terminal
// TypeScriptコンパイラ
$ npx tsc
//  Node.jsとして実行
$ node dist/inde.js
```
