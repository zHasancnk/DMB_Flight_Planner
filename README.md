# Flight_Planner
Hoverfly Aviation Flight Planner System.
Operasyon Merkezi

Bu repo, Operasyon Merkezi paneli olan index.html dosyasını barındırır ve GitHub Pages üzerinden yayınlanır.

Canlı link

https://ORGANIZASYON-ADI.github.io/REPO-ADI/

(Yukarıdaki linki Settings → Pages sayfasından kopyalayıp buraya yapıştırın.)

Sistem nasıl çalışır
Sayfa, 3. sekmedeki "Canlı Rapor" bölümünde bir Google E-Tablo'dan veri çeker.
Veri, Google Form yanıtlarının düştüğü E-Tabloya bağlıdır.
Bağlantı, dosya içindeki CONFIG bölümünden (index.html içinde, en üstlerde) yönetilir:
GOOGLE_SHEET_ID: E-Tablonun adres çubuğundaki ID (https://docs.google.com/spreadsheets/d/BURASI/edit)
GOOGLE_SHEET_GID: Yanıtların olduğu sekmenin numarası (tek sekme varsa 0)
Önemli: Google E-Tablo paylaşım ayarı

E-Tablo, Paylaş → "Bağlantıya sahip olan herkes: Görüntüleyebilir" şeklinde açık kalmalı. Bu kapatılırsa canlı rapor sekmesi hata verir ("Failed to fetch").

Güncelleme yapmak (kod bilmeden)
Bu repoda index.html dosyasına tıklayın.
Sağ üstteki kalem (✎ Edit) ikonuna basın.
Değişikliği yapın (örn. eşik değerleri, form ID, sheet ID).
Sayfanın en altında "Commit changes" butonuna basın.
1-2 dakika içinde canlı sitede güncel hali görünür.
Yeni bir yetkili eklemek
Repo → Settings → Collaborators and teams (Organization kullanıyorsanız: Organization ayarlarından "People" → "Invite member")
Kişinin GitHub kullanıcı adını girip davet gönderin.
Bu repo bir GitHub Organization altında olduğu için, tek bir kişinin ayrılması sistemin erişimini etkilemez — organization'da en az 2 "owner" bulundurulmalıdır.
Sorun giderme
"Failed to fetch" hatası → Google E-Tablo paylaşım ayarını kontrol edin (yukarıya bakın).
Sayfa güncellenmiyor → Tarayıcıda sert yenileme yapın (Ctrl+Shift+R / Cmd+Shift+R), GitHub Pages'in yayılması 1-2 dakika sürebilir.
Yanlış sekmedeki veriler geliyor → GOOGLE_SHEET_GID değerini, ilgili sekmeyi Google Sheets'te açıp adres çubuğundaki gid= değeriyle eşleştirin.
