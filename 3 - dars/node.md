## 1. Type Conversions (Tiplarni o‘zgartirish)

JavaScriptda ma’lumot turlarini bir-biriga o‘zgartirish mumkin. Bu jarayon **type conversion** deb ataladi.

### Misollar:

```js
let son = "123";
let raqam = Number(son); // Stringdan Numberga o‘zgartirish
console.log(raqam); // 123

let qiymat = 456;
let matn = String(qiymat); // Numberdan Stringga o‘zgartirish
console.log(matn); // "456"
```

**Boolean**ga o‘zgartirish:

```js
let qiymat = 0;
let natija = Boolean(qiymat); // false, chunki 0 - false
```

## 2. Operatorlar

Operatorlar yordamida qiymatlar ustida amallar bajariladi.

### Asosiy operatorlar:

- **Qo‘shish (+)**: `a + b`
- **Ayirish (-)**: `a - b`
- **Ko‘paytirish (\*)**: `a * b`
- **Bo‘lish (/)**: `a / b`
- **Qoldiq (%)**: `a % b`

### Misollar:

```js
let a = 10;
let b = 3;
console.log(a + b); // 13
console.log(a % b); // 1
```

## 3. Mantiqiy Amallar (Logical Operations)

Mantiqiy operatorlar yordamida shartlarni tekshirish mumkin.

- **AND (`&&`)**: Ikkala shart ham true bo‘lsa, natija true.
- **OR (`||`)**: Kamida bittasi true bo‘lsa, natija true.
- **NOT (`!`)**: Qiymatni teskarisiga o‘zgartiradi.

### Misollar:

```js
let yosh = 20;
console.log(yosh > 18 && yosh < 30); // true
console.log(yosh < 18 || yosh > 25); // false
console.log(!(yosh == 20)); // false
```
