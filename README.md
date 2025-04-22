# dosyakay-t-file-
input type kısmı ne file diyerek bilgisayardan dosya yüklemeyi yapıyoruz 
   <input type="file"  asp-for="KapakFoto"class="form-control">
form kısmına ise kayıt veri yolu işlemi için
enctype="multipart/form-data"
model kısmında IFormFile? olarak değiştirin resim olarak direk kayıt için 
   [NotMapped] bu alanın veri tabınında olmuyacağı yer
   çünkü dosya klasöre kayıt edilir

   var kokDizini=Directory.GetCurrentDirectory();
   bu komut çalışma klasörünü bulur.
   programın çalıştığı ana dizin (C:\User\Fatih\Desktop\KutuphaneMVC
   
