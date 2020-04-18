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

# Basit bir Thread kodu :

+ Kütüphanelerimizi çağırıyoruz.
Using System;
Using System.Threading;

+ CagirThread adında bir sınıf oluşturduk.

public class CagirThread {
   

   public static void threada(){
        
        for(int x=0; x<10; x++){
          Console.WriteLine(x);
           }
       }
   
    public static void threadb(){

  for(int x=10; x>0; x++){
  Console.WriteLine(x);
       }
   }

}

+ Çalıştırılacak kısım

public class Yürüt {

public static void Main(){

+ İki tane yeni Thread nesnesi oluşturup, başlatıyoruz.

Thread t1 = new Thread(CagirThread.threada);

Thread t2 = new Thread(CagirThread.threadb);

t1.Start();

t2.Start();

}
} 
