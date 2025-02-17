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
### **HTMLda matn bo‘limlarini qanday ajratish mumkin?**  

HTMLda matnni bo‘limlarga ajratish va tartibga solish uchun turli xil teglar ishlatiladi. Quyida eng ko‘p ishlatiladigan usullar bilan tanishamiz:  

---

### **1. `<br>` – Yangi qatordan boshlash (Break Line)**  
Agar matnni yangi qatordan boshlash kerak bo‘lsa, `<br>` tegi ishlatiladi.  
```html
<p>Bu birinchi qator.<br>Bu esa yangi qator.</p>
```
🔹 **Natija:**  
Bu birinchi qator.  
Bu esa yangi qator.  

📌 **Eslatma:** `<br>` tegi o‘z-o‘zidan yopiladi va faqat bitta qator tashlash uchun ishlatiladi.  

---

### **2. `<p>` – Paragraf (Bo‘lim yaratish)**  
Agar matnni alohida bo‘limlarga ajratmoqchi bo‘lsangiz, har bir qismni `<p>` tegi ichiga yozing.  
```html
<p>Bu birinchi paragraf.</p>
<p>Bu esa ikkinchi paragraf.</p>
```
🔹 **Natija:**  
Bu birinchi paragraf.  

Bu esa ikkinchi paragraf.  

📌 **Eslatma:** Brauzer har bir `<p>` tegidan keyin avtomatik ravishda yangi qatordan boshlaydi.  

---

### **3. `<hr>` – Gorizontal chiziq bilan ajratish**  
Matn bo‘limlarini vizual ajratish uchun `<hr>` (Horizontal Rule) tegi ishlatiladi.  
```html
<p>Bu birinchi qism.</p>
<hr>
<p>Bu esa ikkinchi qism.</p>
```
🔹 **Natija:**  
Bu birinchi qism.  
––––––––––––––––––  
Bu esa ikkinchi qism.  

📌 **Eslatma:** `<hr>` tegi o‘z-o‘zidan yopiladi va sahifada gorizontal chiziq hosil qiladi.  

---

### **4. `<div>` – Katta bo‘lim yaratish**  
Agar matnning bir qismini alohida bo‘limga ajratmoqchi bo‘lsangiz, `<div>` tegi ishlatiladi.  
```html
<div style="background-color: #f0f0f0; padding: 10px;">
    <h2>Bo‘lim sarlavhasi</h2>
    <p>Bu bo‘lim ichidagi matn.</p>
</div>
```
🔹 **Natija:**  
Bo‘lim sarlavhasi  
Bu bo‘lim ichidagi matn.  

📌 **Eslatma:** `<div>` ko‘rinmaydi, lekin CSS orqali unga fon, chegaralar va boshqa dizayn elementlari qo‘shish mumkin.  

---

### **5. `<span>` – Matn ichida kichik bo‘lak ajratish**  
Agar faqat bitta so‘z yoki jumlani ajratib ko‘rsatmoqchi bo‘lsangiz, `<span>` tegi ishlatiladi.  
```html
<p>Bu <span style="color: red;">qizil</span> so‘z.</p>
```
🔹 **Natija:**  
Bu **qizil** so‘z.  

📌 **Eslatma:** `<span>` blok yaratmaydi, faqat matn ichidagi alohida qismlarni stil bilan ajratish uchun ishlatiladi.  

---

### **6. `<section>` – Tarkibiy bo‘limlar yaratish**  
Veb-sahifani mantiqiy bo‘limlarga ajratish uchun `<section>` ishlatiladi.  
```html
<section>
    <h2>Bo‘lim sarlavhasi</h2>
    <p>Bu bo‘lim matni.</p>
</section>
```
📌 **Eslatma:** `<section>` tarkibni ma'nosi bo‘yicha ajratish uchun ishlatiladi va SEO uchun foydalidir.  

---

### **7. `<article>` – Mustaqil maqola yoki post yaratish**  
Agar matn mustaqil maqola yoki blog posti bo‘lsa, `<article>` tegi ishlatiladi.  
```html
<article>
    <h2>Maqola sarlavhasi</h2>
    <p>Bu maqolaning matni.</p>
</article>
```
📌 **Eslatma:** `<article>` odatda yangiliklar, blog postlari yoki sharhlar uchun ishlatiladi.  

---

### **Xulosa**  
✅ **Yangi qatordan boshlash:** `<br>`  
✅ **Paragraf yaratish:** `<p>`  
✅ **Chiziq bilan ajratish:** `<hr>`  
✅ **Blok yaratish:** `<div>`  
✅ **Matn ichida ajratish:** `<span>`  
✅ **Bo‘lim yaratish:** `<section>`  
✅ **Maqola yoki post yaratish:** `<article>`  

💡 Qaysi usulni ishlatish kerakligi **matnning qanday maqsadda ajratilishiga bog‘liq**. Agar qo‘shimcha savollaringiz bo‘lsa, bemalol so‘rashingiz mumkin! 😊

### **HTMLda ro‘yxatlar (List types) turlari**  

HTMLda ro‘yxatlar **uch turga** bo‘linadi:  
1. **Tartibsiz ro‘yxat (Unordered List - `<ul>`)**  
2. **Tartibli ro‘yxat (Ordered List - `<ol>`)**  
3. **Tavsifli ro‘yxat (Description List - `<dl>`)**  

---

## **1. Tartibsiz ro‘yxat (`<ul>`)**  
Tartibsiz ro‘yxat (`<ul>`) – bu elementlari oldida belgilar (nuqta, doira, kvadrat) bo‘lgan ro‘yxat.  

### **Misol:**  
```html
<ul>
    <li>Olma</li>
    <li>Banan</li>
    <li>Uzum</li>
</ul>
```
🔹 **Natija:**  
- Olma  
- Banan  
- Uzum  

📌 **`<li>` (List Item)** – har bir ro‘yxat elementini bildiradi.  

### **Belgi turini o‘zgartirish (`type`)**  
```html
<ul type="square">
    <li>Olma</li>
    <li>Banan</li>
    <li>Uzum</li>
</ul>
```
🔹 **Mumkin bo‘lgan qiymatlar:**  
- `disc` (standart nuqta)  
- `circle` (bo‘sh doira)  
- `square` (kvadrat)  

---

## **2. Tartibli ro‘yxat (`<ol>`)**  
Tartibli ro‘yxat (`<ol>`) – bu elementlari **raqamlar yoki harflar bilan** tartiblangan ro‘yxat.  

### **Misol:**  
```html
<ol>
    <li>Birinchi</li>
    <li>Ikkinchi</li>
    <li>Uchinchi</li>
</ol>
```
🔹 **Natija:**  
1. Birinchi  
2. Ikkinchi  
3. Uchinchi  

### **Tartib belgilarini o‘zgartirish (`type`)**  
```html
<ol type="A">
    <li>Birinchi</li>
    <li>Ikkinchi</li>
    <li>Uchinchi</li>
</ol>
```
🔹 **Mumkin bo‘lgan qiymatlar:**  
- `1` → 1, 2, 3, ... (standart)  
- `A` → A, B, C, ...  
- `a` → a, b, c, ...  
- `I` → I, II, III, ...  
- `i` → i, ii, iii, ...  

### **Raqamni belgilangan joydan boshlash (`start`)**  
```html
<ol start="5">
    <li>Beshinchi</li>
    <li>Oltinchi</li>
</ol>
```
🔹 **Natija:**  
5. Beshinchi  
6. Oltinchi  

---

## **3. Tavsifli ro‘yxat (`<dl>`)**  
Tavsifli ro‘yxat (`<dl>`) – bu har bir elementga tavsif qo‘shilgan ro‘yxat.  

### **Misol:**  
```html
<dl>
    <dt>HTML</dt>
    <dd>Veb-sahifalarni yaratish uchun belgilash tili.</dd>

    <dt>CSS</dt>
    <dd>Veb-sahifalarga dizayn berish tili.</dd>
</dl>
```
🔹 **Teglar ma’nosi:**  
- `<dl>` → Description List (Tavsifli ro‘yxat)  
- `<dt>` → Definition Term (Atama yoki sarlavha)  
- `<dd>` → Definition Description (Atamaning tavsifi)  

🔹 **Natija:**  
**HTML**  
Veb-sahifalarni yaratish uchun belgilash tili.  

**CSS**  
Veb-sahifalarga dizayn berish tili.  

---

## **Ichma-ich ro‘yxatlar (Nested Lists)**  
Har qanday ro‘yxatni boshqa ro‘yxat ichiga joylashtirish mumkin.  

### **Misol:**  
```html
<ul>
    <li>Mevalar
        <ul>
            <li>Olma</li>
            <li>Banan</li>
        </ul>
    </li>
    <li>Sabzavotlar
        <ul>
            <li>Sabzi</li>
            <li>Pomidor</li>
        </ul>
    </li>
</ul>
```
🔹 **Natija:**  
- Mevalar  
  - Olma  
  - Banan  
- Sabzavotlar  
  - Sabzi  
  - Pomidor  

---

## **Xulosa**  
✅ **Tartibsiz ro‘yxat (`<ul>`)** → Nuqtalar bilan belgilanadi.  
✅ **Tartibli ro‘yxat (`<ol>`)** → Raqam yoki harflar bilan tartiblanadi.  
✅ **Tavsifli ro‘yxat (`<dl>`)** → Atamalar va ularning tavsiflari ko‘rsatiladi.  
✅ **Ichma-ich ro‘yxatlar** → Ro‘yxat ichida boshqa ro‘yxat bo‘lishi mumkin.  

Agar qo‘shimcha savollaringiz bo‘lsa, bemalol so‘rashingiz mumkin! 😊
