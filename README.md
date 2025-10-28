## 🌟 Tech Stack Focus: State Management (Context API)

Humne iss project mein state management ke liye **React Context API** ka use kiya hai. Yeh ek powerful tool hai jo bade applications mein data sharing ko bahut easy bana deta hai.

---

### ❓ Why Context API? (Prop Drilling Se Chhutkara)

Normally, agar data ko ek parent se bohot saare nested children tak bhejna ho, toh hum props ko har component se manually pass karte hain (jise **Prop Drilling** kehte hain). Context API iss problem ko solve karta hai.

---

### 🌍 Global Access

Context humein ek aisa **global data store** create karne deta hai jise component tree mein koi bhi component directly access kar sakta hai, bina beech ke components ko disturb kiye.

---

### 🪶 Lightweight

**Redux** jaise libraries ke comparison mein, Context API ek **lightweight** aur in-built solution hai jo medium to large-sized applications ke global state ko efficiently handle karta hai.

---

### 🛠️ Implementation Details (Kaise Use Kiya?)

Humne Context ko `useContext` hook ke saath use kiya hai:

* **Context.Provider**: Yeh component top-level par wrap kiya gaya hai (usually `index.js` mein) jisse yeh ensure ho ki global state poore application mein available ho.
* **useContext Hook**: Components mein state ko read aur consume karne ke liye hum `useContext(MyContext)` hook ka use karte hain.

---

### 🧩 Contexts Created

Iss project mein humne mainly:

* **Authentication Status** (login/logout)
* **Application Theme** (Dark/Light mode)

dono ko Context ke through manage kiya hai.

---

### ✅ Quick Flow

`Context.Provider` → App Tree → `useContext` → Consume State

---

### 📌 Conclusion

Context API medium-scale apps ke liye perfect state management solution hai jahan Redux unnecessary heavy ho sakta hai. Yeh clean code, easy access aur better maintainability provide karta hai.
