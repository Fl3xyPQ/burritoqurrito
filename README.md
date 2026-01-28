# 🌸 Radanky Bezpečné Místo

**Speciální interaktivní webová stránka** - platonické bezpečné místo plné povzbuzení, vzpomínek a společných chvil.

---

## 📁 Soubory projektu

```
R jako rachejtle/
├── index.html              ← Hlavní HTML soubor (OTEVŘI TENTO)
├── new-style.css           ← Všechny styly
├── new-script.js           ← Všechna funkcionalita + Firebase
├── FIREBASE-SETUP.md       ← Návod na nastavení Firebase
└── README.md               ← Tento soubor
```

---

## 🚀 Jak spustit

1. **Otevři:** `index.html` v prohlížeči (dvojklik)
2. **Nebo:** Pravý klik → Open with → Chrome/Firefox/Edge
3. **Hotovo!** Web funguje offline (kromě nástěnky)

---

## 🎯 Funkce

### 🏠 **Homepage**
6 mood-based karet podle nálady:
- 💙 Je mi smutno
- 🌊 Jsem naštvaná
- ✨ Chci vzpomínat
- 🎮 Chci se pobavit
- 📝 Chci si něco zapsat
- 🌈 Jen tak navštívit

### 💝 **Útěcha**
- ✨ **Generátor komplimentů** - 16 povzbuzení, counter úsměvů
- 🎁 **Důvody proč jsi úžasná** - Grid karet s důvody
- 💭 **Citáty** - Carousel 5 motivačních citátů
- 💌 **Dopisy "Otevři později"** - 6 obálek s tajnými vzkazy

### ✨ **Vzpomínky**
- 🗓️ **Memory Wall** - Klikací karty se vzpomínkami
- ⏱️ **Počítadlo** - Dny/hodiny/minuty/sekundy od speciálního data
- 🌟 **Konstelace** - Hra na propojování hvězd (1-8)

### 🎮 **Zábava**
- 🧩 **Puzzle** - 4x4 grid tajemného puzzlu
- 🔐 **Tajná zpráva** - Hádanka → odhalí skrytý vzkaz

### 📝 **Poznámky**
- ✍️ **Editor poznámek** - Rychlé poznámky s uložením
- 📋 **Seznam poznámek** - Historie všech poznámek
- 😊 **Mood tracker** - Sledování nálad (6 emocí)
- 📊 **Historie nálad** - Posledních 10 záznamů

### 📌 **Nástěnka** (Vyžaduje Firebase)
- 💌 **Textové vzkazy** - Sticky notes (5 barev)
- 🎨 **Malůvky** - Canvas kreslítko se sdílením
- 🔒 **Přístupový kód** - Soukromá nástěnka jen pro vás dva
- ⚡ **Real-time sync** - Okamžitá synchronizace

---

## 🔧 Nastavení

### 1️⃣ **Základní použití (BEZ Firebase)**
✅ Funguje okamžitě  
✅ Vše kromě nástěnky  
✅ Data v localStorage (pouze toto zařízení)

**Žádné nastavení nepotřeba!**

---

### 2️⃣ **Plná verze (S Firebase)**
Pro funkci **sdílené nástěnky** postupuj podle:

📖 **[FIREBASE-SETUP.md](FIREBASE-SETUP.md)** ← Podrobný návod

**Stručně:**
1. Vytvoř Firebase projekt (5 min)
2. Aktivuj Firestore (2 min)
3. Zkopíruj config do `new-script.js` (1 min)
4. Změň přístupový kód (30 sec)
5. Hotovo! 🎉

---

## 🎨 Customizace

### Změnit přístupový kód k nástěnce:
**Soubor:** `new-script.js`  
**Řádek:** ~111

```javascript
const ACCESS_CODE = "RadankaJirka2026"; // ← ZMĚŇ TOTO
```

### Přidat vlastní komplimenty:
**Soubor:** `new-script.js`  
**Řádky:** 95-111

```javascript
const compliments = [
    "Tvůj vlastní kompliment zde...",
    "Další kompliment...",
    // ... přidej další
];
```

### Změnit citáty:
**Soubor:** `new-script.js`  
**Řádky:** 154-169

### Změnit odpověď na hádanku:
**Soubor:** `new-script.js`  
**Řádek:** ~409

```javascript
const correctAnswer = '42'; // ← Změň odpověď
```

### Upravit texty v HTML:
**Soubor:** `index-new.html`  
**Hledej:** `[Tvůj text zde]` - nahraď vlastním obsahem

### Doplnit dopisy:
**Soubor:** `index-new.html`  
**Řádky:** ~180-230 (sekce s letter-envelope)

---

## ⌨️ Klávesové zkratky

- **Ctrl + 1** → Homepage
- **Ctrl + 2** → Útěcha
- **Ctrl + 3** → Vzpomínky
- **Ctrl + 4** → Zábava
- **Ctrl + 5** → Poznámky

---

## 💾 Data & Úložiště

### LocalStorage (offline):
- Poznámky
- Nálady
- Počet komplimentů
- Speciální datum pro counter

### Firebase (online - volitelné):
- Textové vzkazy
- Malůvky
- Real-time synchronizace

---

## 🎭 Design & Estetika

- **Styl:** Glassmorphism + Organic/Nature
- **Barvy:** Jemné pastelové gradienty
- **Animace:** Smooth transitions (cubic-bezier)
- **Částice:** Floating background particles
- **Responsivní:** Funguje na mobilu i PC

---

## 🌐 Podpora prohlížečů

✅ **Chrome** (doporučeno)  
✅ **Firefox**  
✅ **Edge**  
✅ **Safari**  
✅ **Opera**

**Minimum:** ES6+ support (2015+)

---

## 📱 Mobilní podpora

- ✅ Touch events pro kreslení
- ✅ Responsivní layout
- ✅ Zjednodušená navigace (pouze ikony)
- ✅ Optimalizované pro menší obrazovky

---

## 🆘 Řešení problémů

### Nástěnka se nezobrazuje:
➡️ Zkontroluj přístupový kód  
➡️ Otevři konzoli (F12) - hledej chyby

### Vzkazy se neukládají:
➡️ Zkontroluj Firebase konfiguraci v `new-script.js`  
➡️ Zkontroluj Firestore pravidla (viz FIREBASE-SETUP.md)

### Poznámky zmizely:
➡️ Smazal jsi browser data/cookies?  
➡️ LocalStorage se mažou při "Clear browsing data"  
➡️ **Řešení:** Export/Import funkce (lze přidat)

### Canvas nereaguje:
➡️ Zkus jiný prohlížeč  
➡️ Zkontroluj že JavaScript je povolen

---

## 🚀 Budoucí funkce (návrhy)

- [ ] Export/Import dat
- [ ] Dýchací cvičení pro uklidnění
- [ ] Virtuální objetí s animací
- [ ] Časová kapsula (zprávy do budoucna)
- [ ] Gratitude journal
- [ ] Memory board s fotkami
- [ ] Mini hry (memory, bubble pop)
- [ ] Email notifikace při novém vzkazu

---

## 💖 Pro Radanku

Toto místo je tvoje. Můžeš se sem vrátit kdykoliv potřebuješ:
- Povzbuzení když je ti smutno
- Uklidnění když jsi naštvaná
- Zavzpomínat na krásné chvíle
- Pobavit se hrou
- Zapsat si svoje myšlenky

**Nikdy nejsi sama. 💙**

---

## 📄 Licence

Tato stránka je vytvořena speciálně pro Radanku.  
Pro osobní použití. S láskou vytvořeno. 🌸

---

## 📞 Kontakt

Máš otázku? Něco nefunguje?  
Dej vědět a vyřešíme to! ✨

**Užij si to! 🎉**
