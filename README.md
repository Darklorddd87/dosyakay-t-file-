# dosyakay-t-file-
input type kısmı ne file diyerek bilgisayardan dosya yüklemeyi yapıyoruz 
   <input type="file"  asp-for="Resim"class="form-control">
form kısmına ise kayıt veri yolu işlemi için
enctype="multipart/form-data"
model kısmında IFormFile? olarak değiştirin resim olarak direk kayıt için 

   [NotMapped] 
   
   bu alanın veri tabınında olmuyacağı yer
   
   çünkü dosya klasöre kayıt edilir
   
 if(k.Resim!=null)
 
 eğer boş değilse seçilibirşey varsa
 
   string kokDizini=Directory.GetCurrentDirectory();
   
   bu komut çalışma klasörünü bulur.
   
   programın çalıştığı ana dizin (C:\User\Fatih\Desktop\KutuphaneMVC

    string kayitDizini=Path.Combine(kokDizini,"wwwrot","resim")
    //resmin kayıt edilceği yer belirlendi
    string dosyaAdi=Guid.NewGuid bunla random ad veriyoruz
    
    +Path.GetExtension(k.Resim.FileName); 
    
    ve sonuna buna ekliyerek uzantıyı birebir ekliyoruz
    
    

      var tamYol=Path.Combine(kayitDizini,dosyaAdi);
      
   bu codla seçili belirlenen klasöre kayıt Kayitdizini nere kayıt olacağı ,dosyaAdi ise dosya adi random verip uzantısı aynı 
   using ifadesiyle dosya yüklendikten sonra bellek hemen boşaltılır performans için kullanılır.
    using (var dosyaAkisi=new FileStream(tamYol,FileMode.Create))
    akış oluşturuyor  sadece
      k.Resim.CopyTo(dosyaAkisi);
      burda cop yalayarak dosya kayıt 
       k.KapakFoto=dosyaAdi;
       bura ad kayıt 

       
        if(k.Resim!=null)
        {
        string kokDizini=Directory.GetCurrentDirectory();
         string kayitDizini=Path.Combine(kokDizini,"wwwrot","resim")
         string dosyaAdi=Guid.NewGuid+Path.GetExtension(k.Resim.FileName);
            var tamYol=Path.Combine(kayitDizini,dosyaAdi);
            var dosyaAkisi=new FileStream(tamYol,FileMode.Create)
             k.Resim.CopyTo(dosyaAkisi);
      burda cop yalayarak dosya kayıt 
       k.KapakFoto=dosyaAdi;
         
        
