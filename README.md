<div align="center">

# ARSEN DEVELOPMENT

## Web Panelli Gelişmiş Roleplay Botu

**Discord sunucuları için bot, web yönetim paneli ve karakter portalını tek yapıda birleştiren roleplay altyapısı.**

Discord.js · Next.js · MongoDB · Discord OAuth2 · Components V2

**Aylık 800 TL** &nbsp;·&nbsp; **Tek seferlik 5.000 TL**

</div>

---

## Proje hakkında

ArseN Development tarafından geliştirilen bu paket, Discord üzerindeki metin tabanlı roleplay topluluklarının günlük işleyişini tek bir sistem üzerinden yönetmek için tasarlanmıştır. Sunucu üyeleri Discord komutlarını ve kendilerine ait web ekranlarını kullanırken, yetkililer kayıt, moderasyon, roleplay, ekonomi ve bot ayarlarını merkezi bir panelden yönetebilir.

Paketin örnek uygulaması **Beacon Hills / Teen Wolf** temasıyla hazırlanmıştır. Sunucu kimliği, içerikler, tasarım ve kullanılacak modüller müşteri sunucusunun ihtiyaçlarına göre özelleştirilebilir. Mevcut bot yapısı tek bir Discord sunucusuna göre yapılandırılmıştır; çoklu sunucu altyapısı olarak tanıtılmamaktadır.

## Öne çıkan özellikler

| Sistem | Kapsam |
| :-- | :-- |
| **Web yönetim paneli** | Discord ile giriş, yetkili erişimi, yapılandırma, işlem geçmişi |
| **Roleplay** | RP kategori yönetimi, kelime sayımı, sıralamalar, RP seviye ve ödül sistemi |
| **Ekonomi** | Cüzdan, banka, market, envanter, para transferleri ve işlem kayıtları |
| **Maaş yönetimi** | Rol bazlı maaşlar, haftalık otomatik ödeme, manuel dağıtım ve maaş listesi |
| **Kayıt** | Karakter/üye kayıtları, rol işlemleri ve kayıt bilgileri |
| **Moderasyon** | Ban, kick, mute, jail, uyarı, rol, kanal ve mesaj işlemleri |
| **Guard** | Yetkisiz değişikliklere karşı korumalar, whitelist, olay takibi ve güvenlik kontrolleri |
| **Log sistemi** | Sunucu, moderasyon, ekonomi, RP, Guard, komut, konsol ve web işlem kayıtları |
| **Karakter portalı** | Discord hesabına bağlı karakter, kimlik, RP ve ekonomi verilerini görüntüleme |
| **Topluluk araçları** | AFK, çekiliş, avatar/banner, davet, istatistik ve diğer yardımcı komutlar |

**Arayüz:** Slash komutlar, Discord **Components V2** bileşenleri, uygulama emojileri ve mobil uyumlu **Liquid Glass** web tasarımı.

## Web yönetim paneli

Web portalı, Discord OAuth2 ile giriş yapan kullanıcının sunucu üyeliğini ve yetkilerini kontrol eder. Üyeler kendilerine ait verileri görüntüler; yetkililer erişim düzeylerine uygun yönetim ekranlarını kullanır.

- **Genel bakış:** Topluluk verileri, etkinlik ve sistem durumları.
- **Üye ve karakter yönetimi:** Kayıt, kimlik, ekonomi ve RP bilgileri.
- **Roleplay yönetimi:** Kategoriler, kelime istatistikleri, seviye hedefleri ve ödüller.
- **Ekonomi yönetimi:** Üye bakiyeleri, banka değerleri ve yetkili işlemleri.
- **Bot kurulumu:** Desteklenen kanal/rol eşlemeleri, log ayarları, Guard ve diğer kurulum seçenekleri.
- **Site logları:** Giriş, çıkış ve yönetim işlemlerinin tarihçesi; uygun işlemlerin Discord log kanalına aktarımı.
- **Mobil kullanım:** Telefon ve tablet ekranlarına uyarlanan modern, yarı saydam panel tasarımı.

Web paneli ile bot arasındaki değişiklik talepleri, doğrudan kullanıcı tarayıcısından Discord botuna komut göndermek yerine **yetki kontrollü bir işlem köprüsü** üzerinden yürütülür.

### Rol ve maaş tutarlarını web panelinden yönetme

**Satış paketinde hedeflenen maaş yönetimi** basit, eski rol bazlı düzendir:

1. Yönetici web panelinden bir **Discord rolü** seçer.
2. Rolün **haftalık maaş tutarını** belirler veya değiştirir.
3. İstenmeyen rol–maaş eşlemesini kaldırabilir; güncel listeyi görüntüleyebilir.
4. Bot, ayarlanan maaşları mevcut ekonomi sistemine göre haftalık olarak yatırır.
5. Bir kullanıcı birden fazla maaş tanımlı role sahipse **bu rollerin maaşları toplanır** ve tek ödeme yapılır.
6. Yetkili gerekli olduğunda manuel maaş dağıtımı başlatabilir. Ödemeler ekonomi kayıtlarına işlenir.

**Örnek:** Doktor rolünün haftalık maaşı `750 $`, Öğretmen rolünün maaşı `700 $` olarak ayarlanırsa iki role sahip üye ilgili dağıtımda toplam `1.450 $` alır. Tutarlar örnektir; her sunucuda yönetici tarafından belirlenir.

> **Uygulama durumu:** Eski rol bazlı maaş sistemi botta bulunmaktadır. Web üzerinden **maaşlı rol ekleme, silme ve tutar değiştirme** ekranının botla tam bağlantısı, incelenen eski web sürümünde henüz tamamlanmış değildir. Bu özellik satış paketinin hedef kapsamındadır ve canlı ürün olarak sunulmadan önce tamamlanıp test edilmelidir.

### Maaş modeli hakkında

Bu tanıtım **eski haftalık maaş sistemini** esas alır. Sonradan denenen **600 kelimelik meslek RP'si, mesai anahtar kelimeleri, haftalık üç hak ve yetkili onaylı ödeme** modeli bu ürünün maaş tanımına dahil **değildir**. Maaşlar rol–tutar eşlemelerine göre dağıtılır.

## Kullanıcı deneyimi

### Discord botu

- Tek merkezden erişilen kurulum komutları ve kategori bazlı yönetim.
- Uygulama emojileriyle uyumlu Components V2 arayüzler.
- Metin, ses ve roleplay istatistikleri.
- Karakter kimlikleri ve roleplay odaklı yardımcı özellikler.
- Güvenlik, moderasyon ve işlem kayıtlarının bütünleşik kullanımı.

### Web sitesi

- Roleplay sunucusunun evrenini ve topluluğunu tanıtan açılış sayfası.
- Discord ile güvenli giriş.
- Üyenin karakter ve ekonomi bilgilerinin gösterildiği kişisel panel.
- RP sıralamaları ve karakter arşivi.
- Yetkililere özel yönetim ve log ekranları.
- Masaüstü ve mobil cihazlar için uyarlanmış görünüm.

## Teknik altyapı

| Katman | Teknoloji |
| :-- | :-- |
| Discord botu | JavaScript / Node.js / Discord.js |
| Bot komutları | Slash Commands, Components V2 |
| Web uygulaması | Next.js / React |
| Kimlik doğrulama | Discord OAuth2 |
| Veritabanı | MongoDB |
| Web barındırma | Vercel uyumlu dağıtım |
| Bot barındırma | Sürekli çalışan Node.js sunucusu / VDS |
| Bot–web bağlantısı | MongoDB tabanlı, imzalı ve yetki kontrollü iş kuyruğu |

Hassas yapılandırmalar `.env` ve barındırma servisinin **Environment Variables** bölümünde saklanır. Discord bot tokenı, MongoDB bağlantı bilgileri ve oturum gizli anahtarları GitHub'a eklenmemelidir.

## Paketler ve fiyatlandırma

| Paket | Ücret | Açıklama |
| :-- | --: | :-- |
| **Aylık kullanım** | **800 TL / ay** | Bot ve web panelini aylık kullanım modeliyle edinme |
| **Tek seferlik** | **5.000 TL** | Paket için tek seferlik satın alma seçeneği |

- VDS/barındırma ve paket kapsamındaki özel geliştirmeler için **ayrıca ücret alınmaz**.
- Sunucuya özel görünüm, roller, komut düzeni ve kullanılacak modüller müşteriyle birlikte netleştirilir.
- Teslimat, yönetim erişimi ve destek kapsamı satın alma sırasında karşılıklı belirlenir.
- **Tek seferlik ücret, kaynak kodlarının yeniden satış veya sınırsız dağıtım hakkı verdiği anlamına gelmez.** Lisans koşulları ayrıca belirlenir.

> Fiyatlar Türk lirası cinsindendir. Teklifin kapsamı ve teslim koşulları satın alma öncesinde teyit edilir.

## Örnek proje yapısı

```text
roleplay-platform/
├── bot/
│   ├── src/
│   ├── images/
│   └── data/
└── web/
    ├── app/
    ├── components/
    ├── lib/
    └── public/
```

Bu şema bot ve web uygulamasının **ayrı dağıtıldığını** açıklamak içindir. Gerçek depoda klasörlerin isimleri farklı olabilir. Web sitesi Vercel üzerinde, Discord botu ise sürekli çalışan bir Node.js ortamında barındırılır.

## Kurulum ve güvenlik notları

1. Discord botu için gerekli uygulama yetkileri ve **Gateway Intents** tanımlanır.
2. MongoDB bağlantısı kurulur; bot ve web uygulaması aynı ilgili veritabanı kayıtlarını kullanır.
3. Discord OAuth2 yönlendirme adresi web uygulamasının alan adına göre yapılandırılır.
4. Site ve bot arasındaki yönetim köprüsü için ortak, güvenli bir gizli anahtar belirlenir.
5. Bot kurulum panelinde kanal, rol, log ve Guard ayarları sunucuya göre yapılır.
6. Maaş rolleri ve tutarları tanımlanır; web maaş yönetimi entegrasyonu teslim öncesinde ayrıca doğrulanır.

**Güvenlik ilkesi:** Web panelinde görülen yetki, bot tarafında da yeniden kontrol edilmelidir. Kritik işlemler ve ödeme hareketleri kayıt altına alınmalıdır.

## Lisans ve iletişim

Bu proje **ticari olarak sunulan bir yazılım paketidir**. GitHub'daki tanıtım ve dokümantasyon, kaynak kodlarının ücretsiz kullanımına, kopyalanmasına veya yeniden dağıtılmasına izin verildiği anlamına gelmez.

Satın alma, demo ve sunucuya özel uyarlamalar için **depo sahibi / ArseN Development** ile iletişime geçin.

---

<div align="center">

**ArseN Development**  
*Roleplay toplulukları için Discord botları ve web yönetim sistemleri.*

</div>
