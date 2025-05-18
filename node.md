# Git va GitHub haqida qisqacha dars (Node yozuvi)

## Git nima?

**Git** — bu dasturiy ta'minot ishlab chiqishda kodlarni boshqarish va versiyalarini saqlash uchun ishlatiladigan tizim. U yordamida kod o‘zgarishlarini kuzatish, saqlash va boshqarish mumkin.

## GitHub nima?

**GitHub** — bu Git asosida ishlovchi onlayn platforma. U kodlarni internetda saqlash, ulashish va jamoa bilan ishlash imkonini beradi.

## Asosiy Git buyruqlari

```bash
# Loyihani yangi Git repozitoriyasiga aylantirish
git init

# O'zgartirilgan fayllarni kuzatish uchun qo'shish
git add fayl_nomi

# O'zgartirishlarni saqlash (commit qilish)
git commit -m "Xabar"

# Masofaviy (remote) repozitoriyaga ulanish
git remote add origin https://github.com/foydalanuvchi/repo.git

# O'zgartirishlarni GitHub'ga yuklash
git push -u origin main
```

git clone

## GitHub'da yangi repozitoriya yaratish

1. GitHub saytiga kiring va hisobingizga kiring.
2. "New repository" tugmasini bosing.
3. Repozitoriya nomini kiriting va "Create repository" ni bosing.

## Loyihani GitHub'ga yuklash

1. Terminalda quyidagi buyruqlarni bajaring:

```bash
git init
git add .
git commit -m "Dastlabki commit"
git branch -M main
git remote add origin https://github.com/foydalanuvchi/repo.git
git push -u origin main
```

## Xulosa

Git va GitHub yordamida kodlaringizni boshqarish va jamoa bilan samarali ishlash mumkin. Amaliyotda ko‘proq foydalaning!
