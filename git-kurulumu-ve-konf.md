### **2.1 Git Nasıl Kurulur?**

Git'i resmi sitesinden indir:

🔗 [https://git-scm.com](https://git-scm.com/)

İşletim sistemini otomatik tanır ve uygun dosyayı indirir.

➡️ Kurulum sırasında çıkan adımları **“Next” → “Next” → “Install”** diyerek geçebilirsin.

Varsayılan ayarlar başlangıç için yeterlidir.

---

### **2.2 Kurulum Kontrolü**

Kurulumdan sonra Git’in yüklendiğini doğrulamak için terminal (CMD / PowerShell / Git Bash) aç:

```bash
git --version
```

✅ Çıktı şu şekilde olmalı:

`git version 2.xx.x`

---

### **2.3 Global Ayarlar (Config)**

Git’e kim olduğunu söylemen gerekir. Bu bilgiler, her commit’te görünür:

```bash
git config --global user.name "Adın Soyadın"
git config --global user.email "mail@example.com"
```

Örnek:

```bash
git config --global user.name "Atılay Çetinkaya"
git config --global user.email "atilay@example.com"
```

---

### **2.4 Yapılandırmaları Görüntüleme**

Yapılan ayarları görmek için:

```bash
git config --list
```

Çıktı şu şekilde olur:

```
user.name=Atılay Çetinkaya
user.email=atilay@example.com
```

---

### Ekstra: Git Bash Nedir?

Windows'ta terminal olarak **Git Bash** kullanmanı öneririm.

CMD'den daha gelişmiş ve Linux benzeri komutlar destekler.

Kurulumla birlikte gelir, ayrı indirmen gerekmez.

**CMD Powershel Nedir?**

**CMD (Komut İstemi):** Windows’un klasik komut satırıdır. Temel komutları destekler.

**PowerShell:** CMD’den daha güçlüdür. Nesne tabanlıdır, script yazmaya uygundur. Windows’ta yüklü gelir.

**Git Bash:** Git kurulumuyla gelen özel bir terminaldir. Linux komutlarını destekler. Git işlemleri için daha uygundur.

🟢 Git kullanırken en iyisi: **Git Bash**

Klasik komutlar + Git komutları + Linux benzeri yapı = kolay kullanım

**Terminal Nedir?**

**Terminal**, bilgisayara yazılı komutlar yazarak işlem yaptığın arayüzdür.

Grafik yerine metinle çalışırsın.

🖥️ Örnek işlemler:

- Klasör oluşturmak
- Git komutları çalıştırmak
- Dosya silmek
- Program başlatmak

Windows'ta terminal örnekleri:

- **CMD (Komut İstemi)**
- **PowerShell**
- **Git Bash**

Yani terminal = **yazılı komutlarla bilgisayarı kontrol ettiğin yer**.

**Neden Terminal Kullanırız?**

Çünkü terminal:

✅ **Daha hızlı** → Tek komutla klasör/dosya oluşturabilirsin

✅ **Kodla çalışmaya uygun** → Git, Node.js, React gibi araçlar terminal ister

✅ **Otomasyon sağlar** → Script yazıp işleri otomatikleştirebilirsin

✅ **Sunucu/uzaktan sistemlerde mecburidir** → Sağ tık yoktur

(Uzaktan sistemler: Fiziksel olarak önünde olmayan ama **internet veya ağ üzerinden erişilen** bilgisayarlardır.

Örnekler:

- **VPS (Sanal Sunucu)** – Örn: DigitalOcean, SSDNodes, GüzelHosting
- **Cloud Sunucular** – AWS EC2, Google Cloud VM, Azure
- **Linux Server** – Web siteni barındırdığın sunucular
- **Raspberry Pi** – Evdeki minik bilgisayara SSH ile bağlanmak
- **Uzaktan masaüstü (RDP)** – Başka bir bilgisayara uzaktan bağlanma )

Kısaca: terminal = yazılımcının kontrol paneli 🧠

Grafikle uğraşmak yerine direkt komutla işi halledersin.