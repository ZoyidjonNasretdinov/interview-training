1. What is HTML?
 # interview-training
HTML (HyperText Markup Language) — bu veb-sahifalarni yaratish uchun ishlatiladigan belgilash tili. U sahifaning tuzilishini aniqlaydi va turli elementlar (matn, rasm, tugmalar, havolalar va boshqalar) qanday joylashishini belgilaydi.  

HTML **teglardan** iborat bo‘lib, har bir teg sahifaning ma'lum bir qismini aniqlash uchun ishlatiladi. Masalan:  

```html
<!DOCTYPE html>
<html>
<head>
    <title>Mening birinchi sahifam</title>
</head>
<body>
    <h1>Salom, dunyo!</h1>
    <p>Bu mening birinchi HTML sahifam.</p>
</body>
</html>
```

Yuqoridagi kod oddiy HTML sahifani yaratadi, unda **"Salom, dunyo!"** sarlavhasi va bir parcha matn bor.  

HTML odatda **CSS** (sahifa ko‘rinishini yaxshilash uchun) va **JavaScript** (interaktivlik qo‘shish uchun) bilan birga ishlatiladi.


2. What are HTML tags?
### HTML teglar (tags) nima?  

**HTML teglar** – bu veb-sahifadagi turli elementlarni belgilash uchun ishlatiladigan maxsus kodlar. Har bir HTML elementi **teglar** yordamida boshlanadi va tugaydi.  

### HTML teglarning umumiy tuzilishi:
HTML teglar `< >` belgilari orasiga yoziladi. Ular **ochuvchi teg** va **yopuvchi teg** shaklida bo‘ladi. Masalan:  

```html
<p>Bu paragraf matni.</p>
```

Bu yerda:  
- `<p>` – **ochuvchi teg**  
- `</p>` – **yopuvchi teg**  
- Teglar orasidagi matn esa brauzerda ko‘rinadigan kontentdir.  

### Ba'zi asosiy HTML teglar:  
| Teg | Tavsif |
|------|--------|
| `<h1>` - `<h6>` | Sarlavhalar (h1 eng katta, h6 eng kichik) |
| `<p>` | Paragraf (matn yozish) |
| `<a>` | Havola (link) yaratish |
| `<img>` | Rasm qo‘shish |
| `<ul>` / `<ol>` | Ro‘yxatlar (ul – tartibsiz, ol – tartibli) |
| `<li>` | Ro‘yxat elementi |
| `<div>` | Bo‘lim (blok) yaratish |
| `<span>` | Matn ichida kichik bo‘lak ajratish |
| `<input>` | Forma uchun kiritish maydoni |
| `<button>` | Tugma yaratish |

### Ba'zi HTML teglar yopuvchi tegga ega emas:  
Ba'zi teglar faqat ochuvchi tegdan iborat bo‘ladi, ya’ni ular o‘z-o‘zidan yopiladi. Masalan:  
```html
<img src="rasm.jpg" alt="Bu rasm">
<br>
<hr>
```
- `<img>` – Rasm qo‘shish uchun  
- `<br>` – Yangi qatordan boshlash  
- `<hr>` – Gorizontal chiziq chizish  

**Xulosa:** HTML teglar veb-sahifani yaratish va uning tarkibini belgilash uchun ishlatiladi. Har bir tegning o‘z vazifasi bor va ularning to‘g‘ri ishlatilishi veb-saytning to‘g‘ri ishlashiga yordam beradi. 😊

3. What are HTML Attributes?
### **HTML atributlari nima?**  

**HTML atributlari** – bu teglarning xususiyatlarini belgilash yoki o‘zgartirish uchun ishlatiladigan qo‘shimcha ma'lumotlardir. Atributlar har doim **tegning ochilish qismida** yoziladi va **kalit=qiymat** (`attribute="value"`) shaklida bo‘ladi.  

### **HTML atributlariga misollar**  

#### **1. `href` atributi** (Havola yaratish)  
```html
<a href="https://www.google.com">Google</a>
```
**`href`** atributi `<a>` tegida ishlatiladi va u havolaning manzilini belgilaydi.  

#### **2. `src` atributi** (Rasm qo‘shish)  
```html
<img src="rasm.jpg" alt="Bu rasm tavsifi">
```
**`src`** – rasm manzilini belgilaydi.  
**`alt`** – rasm yuklanmasa, ko‘rinadigan matnni beradi.  

#### **3. `style` atributi** (Elementga stil qo‘shish)  
```html
<p style="color: blue; font-size: 20px;">Bu ko‘k rangdagi matn.</p>
```
**`style`** – elementga CSS orqali dizayn berish uchun ishlatiladi.  

#### **4. `width` va `height` atributlari** (Rasm o‘lchamini belgilash)  
```html
<img src="rasm.jpg" width="200" height="100">
```
**`width`** – rasmning kengligini,  
**`height`** – balandligini piksel (px) yoki foiz (%) bilan belgilaydi.  

#### **5. `id` va `class` atributlari** (Elementlarni tanib olish)  
```html
<p id="mening_matnim">Bu ID bilan belgilangan paragraf.</p>
<p class="matnlar">Bu CLASS bilan belgilangan paragraf.</p>
```
**`id`** – noyob identifikator, odatda JavaScript yoki CSS bilan ishlatiladi.  
**`class`** – bir nechta elementlarga bir xil stil berish yoki ularni tanlash uchun ishlatiladi.  

#### **6. `placeholder` atributi** (Kirish maydoniga tavsiya berish)  
```html
<input type="text" placeholder="Ismingizni kiriting">
```
**`placeholder`** – foydalanuvchiga kiritilishi kerak bo‘lgan ma’lumot haqida ko‘rsatma beradi.  

### **Xulosa**  
- **Atributlar** HTML teglariga qo‘shimcha ma’lumot beradi.  
- **Atributlar har doim ochuvchi tegda yoziladi.**  
- **Kalit=qiymat shaklida bo‘ladi.** (masalan, `href="https://www.google.com"`)  
- **Ko‘pchilik atributlar barcha HTML teglarida ishlatilishi mumkin.**  

Agar qo‘shimcha savollaringiz bo‘lsa, bemalol so‘rashingiz mumkin! 😊

4. What is a marquee in HTML?
### **HTML da `<marquee>` nima?**  

**`<marquee>`** — bu HTML tegi bo‘lib, u matn yoki rasmni ekranda harakatlantirish (skrolling) uchun ishlatiladi. Masalan, matn chapdan o‘ngga, o‘ngdan chapga, yuqoridan pastga yoki pastdan yuqoriga harakat qilishi mumkin.  

📌 **Diqqat!** `<marquee>` tegi HTML5 da eskirgan (deprecated) hisoblanadi va zamonaviy veb-saytlarda **CSS animatsiya yoki JavaScript** ishlatish tavsiya etiladi.

---

### **`<marquee>` ning asosiy ishlatilishi**  

#### **1. Oddiy harakatlanuvchi matn**  
```html
<marquee>Bu harakatlanuvchi matn!</marquee>
```
🔹 Bu matn sukut bo‘yicha **chapdan o‘ngga** qarab harakatlanadi.  

#### **2. Yo‘nalishni o‘zgartirish (`direction`)**  
```html
<marquee direction="right">O‘ng tomonga harakatlanish</marquee>
<marquee direction="up">Yuqoriga harakatlanish</marquee>
<marquee direction="down">Pastga harakatlanish</marquee>
```
🔹 **`direction`** atributi yordamida matnning yo‘nalishini **`left`**, **`right`**, **`up`**, **`down`** qilib o‘zgartirish mumkin.  

#### **3. Tezlikni sozlash (`scrollamount` va `scrolldelay`)**  
```html
<marquee scrollamount="10">Tez harakatlanuvchi matn</marquee>
<marquee scrollamount="2">Sekin harakatlanuvchi matn</marquee>
```
🔹 **`scrollamount`** – tezlikni belgilaydi (katta son – tezroq harakat).  
🔹 **`scrolldelay`** – harakat oralig‘idagi vaqtni belgilaydi (millisekundda).  

#### **4. Cheksiz yoki cheklangan harakat (`loop`)**  
```html
<marquee loop="3">Bu matn faqat 3 marta takrorlanadi.</marquee>
```
🔹 **`loop="3"`** – matn faqat 3 marta harakat qiladi, keyin to‘xtaydi.  
🔹 Agar **`loop="-1"` yoki `loop="infinite"`** ishlatilsa, matn cheksiz davom etadi.  

#### **5. To‘xtash va davom ettirish (`onmouseover` va `onmouseout`)**  
```html
<marquee onmouseover="this.stop();" onmouseout="this.start();">
Sichqoncha ustiga olib kelsangiz, matn to‘xtaydi!
</marquee>
```
🔹 **Sichqoncha matn ustiga kelganda to‘xtaydi, olganda esa davom etadi.**  

---

### **Nega `<marquee>` ishlatish tavsiya etilmaydi?**  
- **`<marquee>` HTML5 da eskirgan (deprecated)** va yangi brauzerlarda to‘liq qo‘llab-quvvatlanmasligi mumkin.  
- Buning o‘rniga **CSS yoki JavaScript** orqali matn yoki rasmni harakatlantirish tavsiya etiladi.  

✅ **CSS orqali matnni harakatlantirish:**  
```css
.marquee {
  white-space: nowrap;
  overflow: hidden;
  display: block;
  animation: move 5s linear infinite;
}

@keyframes move {
  from { transform: translateX(100%); }
  to { transform: translateX(-100%); }
}
```
```html
<div class="marquee">Bu CSS orqali harakatlanuvchi matn!</div>
```

---

### **Xulosa**  
✅ `<marquee>` tegi **matn yoki rasmni harakatlantirish** uchun ishlatiladi.  
❌ Lekin HTML5 da u **eskirgan**, shuning uchun **CSS yoki JavaScript** ishlatish yaxshiroq.  

Agar qo‘shimcha savollaringiz bo‘lsa, bemalol so‘rashingiz mumkin! 😊

