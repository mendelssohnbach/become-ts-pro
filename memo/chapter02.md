# 基本的な文法

## 文と式

`const 変数名 = 式` で構成されたコードが `文`

- 式: 結果がある/計算を行う
- 文: 結果がない/構造を組み立てる
  - 式文: 式を実行するだけ

文=sentence

3 つの文で構成されたプログラム

```TypeScript
const greeting = 'Hello, ';
const target = 'world!';
console.log(greeting + target);
```

式=expression

`Hello, `, `greeting + target`, '+`

式文

`console.log`, `await`, `throw`

## 変数宣言

- 変数宣言: `const 変数名 = 式`
- 変数は 1 つづつ宣言する ','を用いない
- 変数名: 小文字で始める
- 型名: 大文字で始める
- コンポーネント名: 大文字で始める

型注釈:(type annotation): `const 変数: 型注釈 = 式;`

```TypeScript
const greeting: string = 'Hello,';
const repeat: number = 4;
console.log(greeting.repeat(repeat));
```

浮動小数点リテラルの小数部は `e` または `E` で表す

```TypeScript
const small_e = 4e-5;
const large_E = 4e-5;

console.log(small_e, large_E);
// 0.00004,  0.00004
```
