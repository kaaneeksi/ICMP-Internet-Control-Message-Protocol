# ICMP

ICMP’nin temel amacı ağdaki bir bilgisayarın kullanılabilir olup olmadığını, paketlerin bu bilgisayara gidip gelme süresini ve geçtiği bilgisayarların sayısını hesaplamak ve belirlemek için Echo ICMP istek mesajları gönderen Ping veya Trace aracıdır.
**ICMP, sistem yöneticilerine yalnızca rapor verir ve hataları düzeltmez.**

## İleti Türleri

* **Echo Request/Echo Reply (Ping):** Bu tür iletiler, bir ağ cihazından diğerine erişilebilirliği kontrol etmek için kullanılır
  
* **Destination Unreachable:** Bir hedefe ulaşılamadığını belirten iletidir
  
* **Time Exceeded:** Bir paketin belirli bir süre içinde hedefe ulaşamaması durumunda gönderilen bir ilettir.

![ICMP](https://github.com/kaaneeksi/ICMP-Internet-Control-Message-Protocol/blob/main/G%C3%B6rseller/ICMP.jpg)

ICMP'yi bir örnek ile açıklamak gerekirse:

**Ping (Echo Request):**

Bir bilgisayar, hedef bilgisayara bir ICMP Echo Request mesajı gönderir. Bu mesaj, hedef bilgisayarın erişilebilir olup olmadığını kontrol etmek için kullanılır.

Örneğin, bir bilgisayar komut istemcisine şu komutu yazabilirsiniz:

`ping hedef_bilgisayar_ip_adresi`

**Ping (Echo Reply):**

Hedef bilgisayar, ICMP Echo Request mesajını aldığında, bir ICMP Echo Reply mesajı gönderir. Bu, gönderen bilgisayarın hedef bilgisayara erişebildiğini doğrular.

Bu basit örnek, iki bilgisayar arasındaki bağlantıyı kontrol etmek için ICMP'nin nasıl kullanılabileceğini gösterir.

_Burada **Ping** teriminin nereden gelmiş olduğunu öğrenmiş oluyoruz. Kısaca açıklamak istersek:_

 ## Ping
"ping" terimi, genellikle ICMP Echo Request mesajlarını kullanarak bir hedefe ulaşılabilirliği kontrol etmek için yapılan bir ağ aracının adıdır. Yani, "ping" aslında ICMP protokolünü kullanarak bir hedefe Echo Request mesajları gönderme işlemidir. Bu işlem, hedef bilgisayarın erişilebilir olup olmadığını kontrol etmek ve ağ gecikmeyi ölçmek amacıyla yaygın olarak kullanılır.

Yani, temelde "ping" ifadesi, ICMP Echo Request ve Echo Reply mesajlarını kullanarak ağ cihazları arasındaki erişilebilirliği test etmek için kullanılan bir araç veya komutun adıdır. ICMP ise bu işlemin gerçekleştirilmesi için kullanılan protokoldür.

Kısacası, "ping" genellikle ICMP protokolü üzerinde çalışan bir aracın adını ifade eder ve ICMP, bu tür iletişimleri yönetmek için kullanılan protokoldür.
