# Thread-programming-in-CSharp

Thread , bir işlemciye sahip  bilgisayarın işlemci kapasitesi üzerinde programın kendini birçok iş bölümü için 
bölmesine yarar.
Bir nevi zamanı kendi içinde dilimlere ayırması da denilebilir.
Farklı işlemciler üzerinde eş zamanlı çalışması ise bir diğer özelliğidir.

* System.Threading : 
Threading işlemlerini kontrol eden mekanizmalar bu fonksiyonun içerisindedir.

*thread.Start() :
Thread'ı başlatır.

*thread.Sleep() :
Hangi zaman dilimlerinde çalıştırılmasını gerektiğini belirler.

*Thread thread_name = new Thread (new ThreadStart(function1)); : 
Yeni bir thread nesnesi oluşturur.Methodu ise function1 yerine yazılır.

