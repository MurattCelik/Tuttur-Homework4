###Tuttur-Homework2
 
##                                     SHELL'DE MANUEL OLUŞTURMAK 
   
#####       İlk önce nano girmek istediğimiz manuelin adını yazıp manuel sayfasına giriyoruz.Aşağıdaki yazı yazma kurallarına göre manuel sayfasını oluşturuyoruz.
     
 **.TH İSİM BÖLÜM ZAMAN -->>** Bu komutla ana başlık yazılır. Aranılan komutun ve ya dosyanın ismi, hangi bölümde olduğu ve en son değişiklik yapıldığı zaman burada belirtilmektedir.
 
 **.SH  METİN    -->>** Bu komut bölüm başlığı yapmak için kullanılır. Bütün bölümlerin başlığını ("NAME", "SYNOPSIS",  "DESCRIPTION",...vs) yardım (man) sayfasına bu komut yardımı ile yazdırabiliriz. Metin bölümüne hazırlanacak olan bölümün adı yazılır. Eğer metin bölümünde boşluk yoksa tırnak işaretleri kullanılmasına gerek yoktur.
 
 **.SS METİN  -->>** Alt başlık hazırlar. Bu komutla beraber soldan en az 5 karakter boşluk bırakacak şekilde alt başlığı yazdırır. Genel olarak alt başlıkların sadece ilk harfi büyük yazılır. Tekrar **.SH** komutunda olduğu gibi eğer metin bölümünde boşluk yoksa tırnak işaretleri kullanılmasına gerek yoktur.
 
 **.P -->>** Yeni paragraf başlatmak için kullanılır. **"P** komutundan sonraki satırda metin yazılmaya başlanır.
 
 **.IP ÖĞE -->>** Bu komutla daha içerden paragraf başlatılır fakat yazılan öğe bu paragrafın en sol tarafına yani eski paragraf düzenine göre baş tarafa koyulur ve yazılacak  metin daha içeriden başlar. Eğer öğe kısmı boşluk içermiyorsa tırnak kullanımına gerek kalmamaktadır.
 
 **.HP -->>** İç içe paragraf oluşturulmasını sağlar. Yazacağımız metinin 1 satırdan daha uzun olması durumunda ikinci satırın 5 boşluk daha içeriden başlatılmasını sağlar.
 
 **.RE -->>** Satırbaşı yapılmış bir bölgeyi tanımlamaktadır.
 
 **.RS -->>** Paragraf başına göre yazılacak metni 5 boşluk kadar içeriden başlatmaktadır. Metin bu komutun altına yazılır.
 
 **.B METİN -->>** Bu komutla yazılacak olan metin man sayfasına kalın harflerle yazılmaktadır.
 
 **.I METİN -->>** Metinlerin italik yazılmasını sağlar.
 
 **.R -->>**Yazı stili Roman biçiminde yazılır. Genellikle **.IR**(Roman yazı stilinde italik) veya **.BR** (Roman yazı stilinde kalın) şeklinde kullanılır.
 
 **.TP SÜTUN -->>** Yazılacak metne kaç sütun yer ayırılacağı belirtilir. Metin bu komutun altına yazılmaktadır.
 
 **.br -->>** Satırların sonlanadırılmasını sağlar.
 
 **.nf -->>** Normal satır boşluklarını sıkıştırır.
 
 **.fi -->>** Normal satır boşlukları kullanmaya devam edilir. Genelde **.nf** komutundan sonra kullanılır.
 
 **.\" -->>** Yorum satırlarını belirtmek için kullanılır.
  
#####Yaptığımız manuel sayfasını oluşturduktan sonra kaydediyoruz.Daha sonra man dizisine kopyalıyoruz ve ardından zipleyip işlemimizi bitiriyoruz.
    
Örnek olması açısından varsayalım make-star manuel sayfafımızı oluşturduk,kaydettikten sonra aşağıdaki yolu izliyoruz.
 
 **-->> cp** make-star /usr/share/man/man8/.make-star.8 burda kopyalıyoruz  (man dizinimizin yolu nerdeyse orayı seçiyoruz)
 
 **-->> gzip** /usr-/share/man/man8/make-star.8 burda zipliyoruz
 
 ve manulemiz artık hazır  -->> **man make-star**
