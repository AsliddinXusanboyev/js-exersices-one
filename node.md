# JavaScriptda Switch, For loop, While va Do While Looplar

## Switch operatori

switch operatori dasturda takrorlanuvchi yoki ko'p holatli kodlarni soddalashtirish uchun ishlatiladi.

switch - operatori bir nechta holatlarni tekshirish uchun ishlatiladi.

```js
let meva = "olma";

switch (meva) {
  case "olma":
    console.log("Bu olma");
    break;
  case "banan":
    console.log("Bu banan");
    break;
  default:
    console.log("Boshqa meva");
}
```

## For loop

for - biror amalni bir necha marta bajarish uchun ishlatiladi.

```js
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

## While loop

while - shart to'g'ri bo'lsa, doimiy ravishda ishlaydi.

```js
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```

## Do While loop

do while - kamida bir marta bajariladi, keyin shart tekshiriladi.

```js
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 5);
```

