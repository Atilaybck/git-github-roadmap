Branch (dal), projende **paralel geliştirme yapmanı** sağlar. Ana kodu bozmadan yeni özellikler geliştirebilirsin.

### **5.1 `git branch` – Dalları Listele**

Mevcut tüm branch’ları gösterir:

```bash
git branch
```

✅ Çıktıda aktif olduğun branch `*` işareti ile görünür.

---

### **5.2 `git checkout -b yeni-dal` – Yeni Dal Oluştur**

Yeni bir dal oluşturur ve o dala geçer:

```bash
git checkout -b yeni-ozellik
```

📌 Örnek:

```bash
git checkout -b login-formu
```

Bu komut, hem dal oluşturur hem de o dala geçiş yapar.

---

### **5.3 `git checkout branch-ismi` – Dala Geç**

Mevcut bir dala geçmek için:

```bash
git checkout ana-da
```

📌 Örnek:

```bash
git checkout main
```

---

### **5.4 `git merge branch-ismi` – Dal Birleştirme**

Bir dalı, aktif olduğun dala birleştirir:

1. Ana dala geç:
    
    ```bash
    git checkout main
    ```
    
2. Yeni geliştirilen dalı birleştir:
    
    ```bash
    git merge login-formu
    ```
    

✅ Böylece login-formu'ndaki değişiklikler main dalına eklenir.

---

### **5.5 `git branch -d dal-ismi` – Dal Silme**

İşin biten dalı silebilirsin:

```bash
git branch -d login-formu
```

Eğer dal henüz merge edilmediyse, zorla silmek için:

```bash
git branch -D login-formu
```

---

Branch sistemi, büyük projelerde çakışmaları önlemek ve düzenli kod geliştirmek için çok önemlidir.