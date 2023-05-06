Bu repodaki kod parcasi, https://www.tefas.gov.tr/FonAnaliz.aspx?FonKod={FON_ADI} sitesinde, girilen fon ismine gore anlik fiyat bilgilerini ve gunluk degisimlerini cekmektedir. Web scraping yontemi kullanilmaktadir. 

Bir tetikleyici veya baska bir yontem ile SpreadSheet sayfasinda verilerin belirli zaman periyotlarinda guncellenmesini saglayabilirsiniz. 

Fon kisaltmasini girdiginiz hucrenin sag tarafinda fonAnaliz() fonksiyonunu cagirirsaniz, cagirdiginiz hucreye fiyati, bir sagdaki hucreye ise bir onceki gune gore fiyat degisim yuzdesini getirir. 

Sheets'te yeni bir kod sayfasi olusturunuz (.gs uzantisi ile otomatik olusturulur). Bu JavaScript kodunu icerisine kopyalayip kaydettikten sonra fonAnaliz() fonksiyonunu herhangi bir sheets hucrenizde cagirabilirsiniz.

Bu fonksiyonu cagirabilmek icin, kitaplik bolumunde Cheerio kutuphanesini import etmeniz yeterlidir. Cheerio'nun library kodu sudur: 1ReeQ6WO8kKNxoaA_O0XEQ589cIrRvEBA9qcWpNqdOP17i47u6N9M5Xh0

Koddaki bilgiler[index] kismindaki index parametresini degistirerek farkli zaman dilimlerindeki fiyat degisim yuzdelerini de cagirabilirsiniz. Bunun icin fonAnaliz() fonksiyonunun return ettigi diziye, cagiracaginiz ozelligi eklemeniz yeterli olaacaktir.
