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

## 3. Nullish operator (`??`)

Nullish operator qiymat `null` yoki `undefined` bo'lsa, zaxira qiymat beradi.

```js
let ism;
let natija = ism ?? "Ism kiritilmagan";
console.log(natija); // "Ism kiritilmagan"
```

**Xulosa:**

- `if-else` — shartlarni tekshiradi.
- Ternary — qisqa shartli yozuv.
- Nullish (`??`) — qiymat yo'q bo'lsa, zaxira qiymat beradi.
