# Javascript 演習

2024 前期「Javascript 演習」リポジトリ

## 4/15

<h4>オブジェクトの基礎</h4>

```html
<script>
  const dict = { apple: "りんご", banana: "バナナ", orange: "オレンジ" };
  console.log(dict.apple);
  console.log(dict["apple"]);
  dict.apple = "林檎";
  console.log(dict.apple);
  dict.grape = "ぶどう";
  console.log(dict);

  delete dict.orange;
  console.log(dict);
</script>
```

<h4>クラス定義</h4>

```js
//クラスの定義
class InstantNoodle {
  constructor(ramen, taste) {
    this.name = ramen;
    this.soup = taste;
  }
  // メソッドを入れる場合はより便利
  descript() {
    return `<p>${this.name}は、${this.soup}味です</p>`;
  }
}

const soltRamen = new InstantNoodle("サッポロ一番", "塩");
const demae = new InstantNoodle("出前一丁", "醤油");
console.log(soltRamen);
console.log(`${soltRamen.name}は${soltRamen.name}味です`);
console.log(demae);
console.log(`${demae.name}は、${demae.soup}味です`);
```

```js
//クラスの定義;
class InstantNoodle {
  constructor(ramen, taste) {
    this.name = ramen;
    this.soup = taste;
  }
  // メソッドを入れる場合はより便利
  descript() {
    return `<p>${this.name}は、${this.soup}味です<p/>`;
  }
}

const soltRamen = new InstantNoodle("サッポロ一番", "塩");
const demae = new InstantNoodle("出前一丁", "醤油");

//関数の実行;
document.body.insertAdjacentHTML("beforeend", soltRamen.descript());
document.body.insertAdjacentHTML("beforeend", demae.descript());
```
