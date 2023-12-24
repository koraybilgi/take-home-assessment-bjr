# Take-Home Assesment

## Prosedür
- Bu görev için bir github reposu açın ve görev bitiminde adresini paylaşın.
- Görevin tamamlanacağı yazılım dili Golang ve framework Buffalo'dur.
- Veritabanı, kuyruk vb. 3.ncü parti araçlar için teknoloji tercihi sınırlaması yoktur.
- Dış kaynaklardan faydalanmanız durumunda lütfen kullandığınız kaynakları görev içerisinde yorum olarak belirtin.
- Görev için bir zaman sınırlaması yoktur.

## Veriler
Örnek JSON dosyalarına [example-data](./example-data) klasöründen ulaşabilirsiniz.

## Platform (*Opsiyonel*)
Görev içeriği Docker platformu üzerinde ayağa kaldırılıp test edilebilmelidir.

## Sorularınız Varsa
Görevle ilgili sorularınız varsa lütfen iletişime geçmekten çekinmeyin.

---

## Görev 1: Aktiviteler
Aktiviteler için ekleme / silme / listeleme işlemlerinin gerçekleştirilebileceği bir **RESTful** API servisi oluşturun.

### Aktivite Kuralları
- Her aktivite bir profile bağlıdır.
- Aktivite aksiyon türleri (**activities.action**) yalnızca "browsed", "watched", "played" olabilir.
- Ekleme işlemi sırasında tüm payload için validasyon gerçekleştirin.

### Örnek Data:
- [activities.json](./example-data/activities.json)
- [profiles.json](./example-data/profiles.json)

---

## Görev 2: Authentication
Uygulamanız için bir JWT authentication mekanizması oluşturun.

---

## Görev 3: Socket.io
Bir socket.io sunucusu oluşturun. Socket client'larının activities endpoint'ine kayıt eklemesine olanak sağlayın.

### Socket.io Kuralları
- Socket.io sunucusu REST sunucusu ile aynı authentication mekanizmasını kullanır. Bir token her iki serviste de valid ya da invalid'dir.
