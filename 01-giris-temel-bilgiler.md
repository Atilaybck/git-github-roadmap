### **1.1 Git nedir?**

**Git**, bir **versiyon kontrol sistemidir (VCS - Version Control System)**.

Yani, bir projede yaptığın değişiklikleri adım adım takip eder, önceki sürümlere dönmeni sağlar ve aynı anda birçok kişiyle çakışmadan çalışmanı mümkün kılar.

✅ Kısaca:

- Hangi dosya ne zaman, kim tarafından, nasıl değişti → *hepsini takip eder.*
- Gerektiğinde önceki haline dönebilirsin.
- Başkalarıyla aynı projede çalışırken değişiklikleri birleştirebilirsin.

### **1.2 GitHub nedir?**

**GitHub**, Git ile yönetilen projeleri **uzaktan barındıran bir platformdur.**

Yani Git ile çalıştığın dosyaları **internette saklamak**, başkalarıyla paylaşmak ve birlikte geliştirmek için kullanılır.

✅ GitHub bir Git değildir. Git bir sistemdir; GitHub ise bu sistemi barındıran bir web servisidir.

(Alternatifleri: GitLab, Bitbucket)

### **1.3 Versiyon Kontrol Sistemi (VCS) nedir?**

VCS, yazılım geliştirme sürecinde:

- Yapılan tüm değişiklikleri kayıt altına alır,
- Önceki sürümlere geri dönmeyi sağlar,
- Aynı proje üzerinde birden fazla geliştiricinin çakışmadan çalışmasını mümkün kılar.

Git, **dağıtık bir VCS’dir**.

Yani herkesin kendi bilgisayarında tam bir proje kopyası bulunur (sadece sunucuda değil).

### **1.4 Git ve GitHub farkı nedir?**

| Git | GitHub |
| --- | --- |
| Komut satırıyla kullanılır | Web platformudur |
| Versiyon takibini yapar | Kodları internet üzerinde saklar |
| Local çalışır | Remote çalışır (bulut) |
| GitHub olmadan kullanılabilir | Git olmadan çalışmaz |

### **1.5 Local Repo ve Remote Repo farkı nedir?**

- **Local Repo:** Bilgisayarındaki proje klasörü (örneğin `C:\Projeler\cloki-app`)
- **Remote Repo:** GitHub’da barındırılan proje (örneğin `https://github.com/kullanici/cloki-app`)

İlk olarak local’de çalışırsın. Sonra `git push` komutuyla bu değişiklikleri GitHub’daki (remote) repoya yollarsın.

**Repo Ne Demek?**

**Repo** (repository), bir projenin tüm dosyalarını ve bu dosyaların geçmişini (versiyonlarını) tutan yerdir.

Yani projenin kaynak kodu + değişiklik geçmişidir.

Özetle:

**Repo = Proje + Versiyon Geçmişi**