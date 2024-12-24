# İçecek Otomatı Uygulaması - README

## Proje Hakkında
Bu proje, kullanıcıların içecekleri seçip, toplam tutarı görüntüleyip satın alma işlemi yapabileceği basit bir içecek otomatı uygulamasıdır. Tkinter kütüphanesi kullanılarak geliştirilmiştir. Uygulama, içeceklerin fiyatlarını gösterir ve kullanıcılar içecek seçtikçe toplam tutar güncellenir. Satın alma işlemi tamamlandıktan sonra, toplam tutar sıfırlanır ve kullanıcıya bilgi verilir.

## Özellikler
- Kullanıcı, belirli içecekleri (Kahve, Çay, Ayran, Kola, Su) seçebilir.
- Seçilen içeceklerin fiyatları otomatik olarak toplam tutara eklenir.
- "Satın Al" butonuna tıklayarak, seçilen içeceklerin toplam fiyatı gösterilir ve işlem tamamlanır.
- Kullanıcı içecek seçmeden "Satın Al" butonuna tıkladığında, bir uyarı mesajı gösterilir.

## Kullanım
1. Programı çalıştırdığınızda, bir pencere açılacaktır.
2. Pencere üzerinde içecekler ve fiyatları yer alacak.
3. Bir içecek seçmek için, ilgili butona tıklayın. Seçtiğiniz içecek, toplam tutara eklenir.
4. Tüm seçimlerinizi yaptıktan sonra, "Satın Al" butonuna tıklayın. Toplam tutar ve işlem hakkında bilgi veren bir mesaj kutusu görünecektir.
5. Eğer herhangi bir içecek seçilmeden "Satın Al" butonuna tıklanırsa, bir uyarı mesajı alırsınız.

## Gereksinimler
- Python 3.x
- Tkinter kütüphanesi (Python ile birlikte gelir)

## Kod Açıklaması

### İçecekler
`beverages` sözlüğü, mevcut içecekleri ve fiyatlarını içerir:
```python
beverages = {
    "Kahve": 5.0,
    "Çay": 3.0,
    "Ayran": 4.0,
    "Kola": 6.0,
    "Su": 2.0
}
```

### Otomat Sınıfı
`BeverageVendingMachine` sınıfı, uygulamanın ana işlevlerini barındırır:
- **select_beverage**: Kullanıcının seçtiği içeceği ve fiyatını toplam tutara ekler.
- **purchase**: Satın alma işlemini gerçekleştirir ve toplam tutar sıfırlanır.

### Tkinter Arayüzü
- **Label**: Uygulama başlığı ve toplam tutar.
- **Button**: İçeriklerin seçilmesi ve satın alma işlemi için butonlar.
- **messagebox**: Kullanıcıya bilgi ve uyarı mesajları göstermektedir.

## Kurulum ve Çalıştırma
1. Python yüklü değilse, [Python İndirme Sayfası](https://www.python.org/downloads/) üzerinden Python'u indirin.
2. Uygulamayı çalıştırmak için aşağıdaki komutları kullanabilirsiniz:
   ```bash
   python otomat.py
   ```

## Lisans
Bu proje, MIT Lisansı altında lisanslanmıştır.
