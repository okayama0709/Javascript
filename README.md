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

```
