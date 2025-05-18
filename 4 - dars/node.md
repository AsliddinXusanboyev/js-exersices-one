# JavaScript: `if-else`, Ternary Operator va Nullish Operator

## 1. `if-else` operatori

`if-else` yordamida shartlarni tekshirish va turli kodlarni bajarish mumkin.

```js
let yosh = 18;

if (yosh >= 18) {
  console.log("Siz balog'at yoshidasiz.");
} else {
  console.log("Siz balog'at yoshida emassiz.");
}

let a = "maktab xovlisi";

if (a == "maktab xovlisi") {
  console.log(true);
} else {
  console.log(false);
}
```

## 2. Ternary operator (`? :`)

Ternary operator qisqa yozuv uchun ishlatiladi.

```js
let yosh = 18;
let natija = yosh >= 18 ? "Balog'at yoshida" : "Balog'at yoshida emas";
console.log(natija);
```


**Xulosa:**

- `if-else` — shartlarni tekshiradi.
- Ternary — qisqa shartli yozuv.
