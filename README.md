## RSA Metin Şifreleyici

Java, Spring (2016)

* [jar dosyası](http://bit.ly/2oMzZ9P)

**1.** _P ve Q seçilen bit uzunluğunda olmak üzere, birbirinden farklı iki asal sayı hesaplanır._

**2.** _N = P \* Q hesaplanır._

**3.** _ϕ(N) = (P − 1) \* (Q − 1) hesaplanır._

**4.** _ebob(ϕ(N), E) = 1 olacak şekilde E sayısı hesaplanır._

**5.** _E \* D = 1 (mod ϕ(N)) olacak şekilde D sayısı hesaplanır._

N ve E açık anahtarlarken, N ve D gizli anahtarlardır.

N ve E anahtarları metni şifrelerken kullanılır.

N ve D anahtarları şifreli metni çözümlerken kullanılır.

![](https://1.bp.blogspot.com/-nZYxp-mbqZ8/WprlKq7gsnI/AAAAAAAAAHo/Z8Q2cwZDbksZa4E_Z1Ln7bBOqtGAghQ2wCLcBGAs/s1080/1.png)

_Girilen metnin byte değeri (byte değer)^E (mod N) formülü ile şifrelenerek şifrelenmiş metnin byte değeri elde edilir. Bu değer Base64 olarak gösterildi._

![](https://4.bp.blogspot.com/-BP_2hJAY_m8/WprlKkAHTnI/AAAAAAAAAHk/dsf1mi0yIXAOl3PYP4CVNtgdac9mcRQuACLcBGAs/s1080/2.png)

_Şifreli metnin Base64 değeri byte çevrilir, (byte değer)^D (mod N) formülü ile orjinal metnin byte değeri elde edilir. Bu değer char dizisine aktarılarak orjinal metin elde edilir._

![](https://3.bp.blogspot.com/-tA6jKUMBbOw/WprlKSVPqcI/AAAAAAAAAHg/TY4eJUtzkmE3sV5POW2hbtKeVh3BqD4BACLcBGAs/s1080/3.png)

_D veya N değerini 1 azaltmak bile şifreli metnin çözümlenmesini imkansız hale getirir._

![](https://4.bp.blogspot.com/-I5Syqw0SHFs/WprlLHT3pwI/AAAAAAAAAHs/TDAhNTucgnEjRTDVSnovBxqak2XYuHD5ACLcBGAs/s1080/4.png)
