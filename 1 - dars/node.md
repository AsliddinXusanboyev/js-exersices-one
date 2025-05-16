## JavaScript - birinchi nomi LifeScript bo`lgan kyn chalik EcmaScript bolgan

## `Compile` qilish uchun uch xil usul bor

                1)online
                2)browser
                3)node

## Node yuklab olish uchun - node.js ning asosiy web sitega kirib yuklaymiz `Linux`ga yuklangan bo`ladi

# JavaScript O'zgaruvchilar (Variables )

JavaScriptda o'zgaruvchilar ma'lumotlarni saqlash uchun ishlatiladi. O'zgaruvchilarni e'lon qilish uchun :
var, let yoki const -- kalit so'zlari ishlatiladi.

## O'zgaruvchilarni e'lon qilish

### var

var eski usulda o'zgaruvchilarni e'lon qilish uchun ishlatiladi. U global yoki funksiya doirasida amal qiladi.

var ism = "Ali";
console.log(ism);

### let

let blok doirasida amal qiladi va hozirgi zamonaviy JavaScriptda tavsiya etiladi.

javascript
let yosh = 25;
console.log(yosh);

### const

const o'zgarmas qiymatlarni e'lon qilish uchun ishlatiladi. Bir marta qiymat berilgandan keyin uni o'zgartirib bo'lmaydi.

javascript
const PI = 3.14;
console.log(PI);

## Xulosa

- var eski usul, global yoki funksiya doirasida ishlaydi.
- let blok doirasida ishlaydi va zamonaviy usul hisoblanadi.
- const o'zgarmas qiymatlar uchun ishlatiladi.

O'zgaruvchilarni to'g'ri tanlash kodni tushunarli va samarali qiladi.

## JavaScript Ma'lumot Turlari (Data Types)

JavaScriptda ma'lumot turlari ikkiga bo'linadi: Primitive va Non-Primitive.

### Primitive Ma'lumot Turlari

Primitive ma'lumot turlari oddiy qiymatlarni ifodalaydi va quyidagilarni o'z ichiga oladi:

1. String  
   Matnli qiymatlarni ifodalaydi. Ikkita yoki bitta qo'shtirnoq ichida yoziladi.

   let ism = "Ali";
   let salom = 'Salom';
   console.log(ism, salom);

2. Number  
   Butun yoki o'nlik sonlarni ifodalaydi.

   let yosh = 25;
   let pi = 3.14;
   console.log(yosh, pi);

3. Boolean  
   Mantiqiy qiymatlarni ifodalaydi: true yoki false.

   let rost = true;
   let yolg'on = false;
   console.log(rost, yolg'on);

4. Undefined  
   Qiymat berilmagan o'zgaruvchini ifodalaydi.

   let x;
   console.log(x); // undefined

5. Null  
   Bo'sh yoki mavjud bo'lmagan qiymatni ifodalaydi.

   let y = null;
   console.log(y); // null

6. Symbol  
   Unikal va o'zgarmas qiymatlarni yaratish uchun ishlatiladi.

   let symbol = Symbol('unique');
   console.log(symbol);

7. BigInt  
   Juda katta butun sonlarni ifodalaydi.

   `Number.MAX.SAFE.INTAGER
   Number.MIN.SAFE.INTAGER`

   let kattaSon = 96385274100147258369n;
   console.log(kattaSon);

### Non-Primitive Ma'lumot Turlari

Non-Primitive ma'lumot turlari murakkab tuzilmalarni ifodalaydi:

1. Object  
   Kalit-qiymat juftliklarini saqlash uchun ishlatiladi.

   let talaba = {
   ism: "Ali",
   yosh: 25
   };
   console.log(talaba);

2. Array  
   Bir nechta qiymatlarni bitta o'zgaruvchida saqlash uchun ishlatiladi.

   let sonlar = [1, 2, 3, 4, 5];
   console.log(sonlar);

3. Function  
   Kod bloklarini qayta ishlatish uchun ishlatiladi.

   function salomBer() {
   console.log("Salom!");
   }
   salomBer();

## Xulosa

JavaScriptda ma'lumot turlarini to'g'ri tanlash kodni samarali va tushunarli qiladi. Primitive turlar oddiy qiymatlar uchun, non-primitive turlar esa murakkab tuzilmalar uchun ishlatiladi.

## JavaScriptda Xotira Boshqaruvi: Stack va Heap

JavaScriptda xotira boshqaruvi ikkita asosiy tuzilma orqali amalga oshiriladi: Stack va Heap. Ushbu tuzilmalar ma'lumotlarni saqlash va ularga kirishni samarali boshqarish uchun ishlatiladi.

### Stack (Stek)

Stack - bu ma'lumotlarni tartib bilan saqlash uchun ishlatiladigan tezkor va cheklangan xotira tuzilmasi. U LIFO (Last In, First Out) tamoyiliga asoslangan, ya'ni oxirgi qo'shilgan ma'lumot birinchi bo'lib o'chiriladi.

#### Stackning xususiyatlari:

1. Statik xotira: O'lchami oldindan belgilangan va o'zgarmaydi.
2. Tezkor: Ma'lumotlarni yozish va o'qish juda tez amalga oshiriladi.
3. Primivite turlarni saqlash: String, Number, Boolean kabi oddiy qiymatlar stekda saqlanadi.
4. Funksiya chaqiruvlari: Funksiya chaqiruvlari va mahalliy o'zgaruvchilar stekda boshqariladi.

#### Misol:

function hisobla(a, b) {
let natija = a + b; 
}
hisobla(5, 10);

Yuqoridagi misolda a, b va natija o'zgaruvchilari stekda saqlanadi va funksiya chaqiruv tugagach, ular avtomatik ravishda xotiradan o'chiriladi.

---

### Heap (Xip)

Heap - bu murakkab va dinamik ma'lumotlarni saqlash uchun ishlatiladigan xotira tuzilmasi. U strukturaviy ma'lumotlar (masalan, obyektlar va massivlar) uchun ishlatiladi.

#### Heapning xususiyatlari:

1. Dinamik xotira: O'lchami oldindan belgilangan emas va kerak bo'lganda kengaytiriladi.
2. Sekinroq: Ma'lumotlarni yozish va o'qish stekka qaraganda sekinroq.
3. Non-Primitive turlarni saqlash: Object, Array, Function kabi murakkab tuzilmalar xipda saqlanadi.
4. Garbage Collection: JavaScript avtomatik ravishda foydalanilmayotgan ma'lumotlarni xipdan o'chiradi.

#### Misol:

let talaba = {
ism: "Ali",
yosh: 25
}; // 'talaba' xipda saqlanadi

Yuqoridagi misolda talaba obyektining qiymatlari xipda saqlanadi, lekin unga ishora qiluvchi o'zgaruvchi (talaba) stekda joylashadi.

---

### Stack va Heap o'rtasidagi farqlar

| Xususiyat                | Stack                              | Heap                      |
| ------------------------ | ---------------------------------- | ------------------------- |
| Xotira turi              | Statik                             | Dinamik                   |
| Tezlik                   | Tez                                | Sekin                     |
| Saqlanadigan ma'lumotlar | Primitive turlar                   | Non-Primitive turlar      |
| Xotira boshqaruvi        | Avtomatik (funksiya tugashi bilan) | Garbage Collection orqali |

---

### Xotira muammolari

1. Memory Leak (Xotira oqishi): Foydalanilmayotgan obyektlar xipda qolib ketishi mumkin.

   let globalObj = {};
   function addData() {
   globalObj.data = new Array(1000000).fill("data");
   }
   addData(); // 'data' xotiradan o'chirilmaydi

2. Stack Overflow: Juda ko'p rekursiv chaqiruvlar stekni to'ldirib yuborishi mumkin.

   function rekursiya() {
   rekursiya(); // Stack Overflow xatosi
   }
   rekursiya();

---

### Xulosa

- Stack tezkor va oddiy qiymatlar uchun ishlatiladi.
- Heap murakkab tuzilmalar uchun ishlatiladi.
- Xotira boshqaruvini tushunish samarali va optimallashtirilgan kod yozishga yordam beradi.
- Garbage Collection JavaScriptda xotira boshqaruvini avtomatlashtiradi, lekin xotira oqishining oldini olish uchun ehtiyot bo'lish kerak.
