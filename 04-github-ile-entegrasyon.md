Git ile yerelde oluşturduğun projeyi GitHub’a yüklemek için bu adımları takip et.

### **4.1 GitHub Hesabı Oluştur**

- GitHub resmi sitesi: [https://github.com](https://github.com/)
- Ücretsiz hesap oluştur (e-posta doğrulaması gerekir)
- Profil bilgilerini düzenleyebilirsin (fotoğraf, bio vs.)

---

### **4.2 Yeni Repo Oluştur**

GitHub’a giriş yaptıktan sonra:

1. Sağ üstten **"+" → "New repository"** seç
2. Repo ismini yaz (örneğin: `cloki-app`)
3. "Public" veya "Private" seç (tercihine göre)
4. README dosyası **ekleme** (çünkü local projenle çakışabilir)
5. **"Create repository"** butonuna bas

✅ GitHub sana bir bağlantı verecek, şöyle:

```
https://github.com/kullaniciadi/cloki-app.git
```

---

### **4.3 Remote Bağlantısı Ekle**

Local projenin içine git (`cd klasorAdi`) ve şu komutu yaz:

```bash
git remote add origin https://github.com/kullaniciadi/cloki-app.git
```

✅ Bu, GitHub’daki repoyu local proje ile bağlar.

Artık bu bağlantıya `origin` diyebilirsin.

Yani:

**`git remote add origin ...`** demek:

“GitHub’daki repoyu, bilgisayarımdaki projeye bağla” demektir.

🔗 `remote` → uzak sunucu (GitHub)

📝 `origin` → GitHub bağlantısına verdiğimiz takma isim

📌 `add` → bu bağlantıyı ekle

Bunu **sadece ilk sefer** yaparsın, yani:

### 🔁 Akış şu:

1. Bilgisayarında proje klasörünü oluşturdun
2. Git ile başlattın: `git init`
3. GitHub’da repo açtın
4. **Bir kere** `git remote add origin ...` yazdın → bağlantı kuruldu ✅
5. Sonra her push’ta sadece şu yeter:
    
    ```bash
    git push origin master
    ```
    

Yani `git remote add origin` = **ilk tanıştırma**

Sonraki push’lar artık direkt gider.

Devam edelim mi `git`

---

### **4.4 İlk Push (Yükleme)**

Şimdi projenin GitHub’a yüklenmesi için:

```bash
git push -u origin main
```

> Eğer main yerine master kullanıyorsan:
> 

```bash
git push -u origin master
```

✅ `-u` parametresi, bundan sonra sadece `git push` demen yeterli olsun diye kullanılır.

**`master`** ve **`main`**, Git’teki **varsayılan ana dal (branch)** ismidir.

### 🔁 Fark:

- Eskiden: `master` varsayılan daldı
- Günümüzde: GitHub ve Git artık `main` ismini varsayılan yaptı
    
    (daha kapsayıcı ve tarafsız dil için)
    

### 🛠 Sen ne kullanmalısın?

- GitHub’daki repo `main` olarak açıldıysa → `main`
- Eğer projen eskiyse veya sen elle `master` olarak başlattıysan → `master`

🧠 Kısaca:

Aynı şeydirler, sadece isim farkı vardır.

**Dal (branch)**, projenin bir **versiyonunun ayrı bir kopyasıdır.**

🧠 Şöyle düşün:

Ana yol → `main` veya `master`

Yan yol → Yeni bir özellik için ayrı dal (örnek: `login-page`)

Sen bu yan yolda değişiklik yaparsın, ana yola zarar gelmez.

İşin bitince birleşme yapılır (merge).

📦 Özetle:

**Dal = projenin bağımsız bir çalışma kopyası**

---

Artık GitHub sayfana giderek projenin oraya yüklendiğini görebilirsin.