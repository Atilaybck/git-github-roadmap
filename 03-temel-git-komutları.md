- **3. Temel Git Komutları**
    
    Bu bölümde, bir projede en çok kullanacağın temel komutları öğreneceksin.
    
    ### **3.1 `git init` – Yeni Repo Başlatma**
    
    Bir klasörde Git takibini başlatır.
    
    ```bash
    git init
    ```
    
    ✅ Bu komut çalıştığında klasöre `.git` adında gizli bir klasör eklenir.
    
    Artık o klasör bir **Git reposudur** ve tüm değişiklikler takip edilebilir.
    
    ---
    
    ### **3.2 `git status` – Durum Kontrolü**
    
    Hangi dosyaların değiştiğini, hangilerinin eklenmediğini gösterir.
    
    ```bash
    git status
    ```
    
    ✅ Her değişiklikten sonra `git status` ile durumu kontrol etmek iyi alışkanlıktır.
    
    ---
    
    ### **3.3 `git add` – Değişiklikleri Stage Etme**
    
    Git, değişiklikleri doğrudan kaydetmez. Önce "sahneye" (stage) alırsın:
    
    ```bash
    git add dosyaadi.txt
    ```
    
    Tüm dosyalar için:
    
    ```bash
    git add .
    ```
    
    **Stage etmek**, yaptığın değişiklikleri **Git’e "şimdilik kaydet" demektir**, yani commit öncesi hazırlık aşamasıdır.
    
    🧠 Benzer düşün:
    
    - Word belgesine yazdın → **henüz kaydetmedin**
    - "Kaydet" demeden önce "ön izleme alanı" gibi
    
    👉 `git add` → Git’e “bu dosyayı bir sonraki commit’e dahil et” dersin.
    
    👉 `git commit` → Artık o değişikliği kalıcı olarak versiyon geçmişine eklersin.
    
    Yani:
    
    **Çalış → `git add` → `git commit`**
    
    **Neden direkt commit etmiyoruz stage ediyoruz?**
    
    Çünkü **her değişikliği commit etmek istemeyebilirsin**. Stage etmek sana kontrol sağlar.
    
    Örnek senaryo:
    
    3 dosyada değişiklik yaptın ama sadece 1 tanesini kaydetmek istiyorsun.
    
    ✅ `git add dosya1.js` → sadece onu stage ettin
    
    ✅ `git commit -m "buton rengi düzeltildi"` → sadece o değişiklik kaydedilir
    
    Yani:
    
    🟢 **Stage = neyi commit edeceğini seçme aşaması**
    
    🔒 **Commit = seçilenleri kalıcı olarak kaydetme**
    
    Bu sayede commit geçmişin daha temiz ve anlamlı olur.
    
    ---
    
    ### **3.4 `git commit` – Kaydetme (snapshot)**
    
    Stage’e aldığın dosyaları **"commit"** ederek versiyon kaydı oluşturursun:
    
    ```bash
    git commit -m "Açıklayıcı commit mesajı"
    ```
    
    📝 Örnek:
    
    ```bash
    git commit -m "Login sayfası tasarlandı"
    ```
    
    ---
    
    ### **3.5 `git log` – Geçmişi Görüntüleme**
    
    Tüm commit geçmişini gösterir:
    
    ```bash
    git log
    ```
    
    Çıktı örneği:
    
    ```sql
    commit 1a2b3c4d...
    Author: Atilay <atilay@example.com>
    Date:   2025-05-05
    
        Login sayfası tasarlandı
    
    commit 5d6e7f8g...
    Author: Atilay <atilay@example.com>
    Date:   2025-05-04
    
        Proje başlatıldı
    
    ```
    
    ---
    
    ### **3.6 `git diff` – Farkları Görme**
    
    Henüz commit edilmemiş değişiklikleri gösterir:
    
    ```bash
    git diff
    ```
    
    Stage’e alınan ve alınmayan değişiklikleri ayrı ayrı da görebilirsin:
    
    ```bash
    git diff --staged
    ```
    
    ---
    
    🔁 **Özet Akış:**
    ```bash
    git init
    git status
    git add .
    git commit -m "ilk kayıt"
    ```