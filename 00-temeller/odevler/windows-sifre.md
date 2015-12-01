# Kali Linux ile Windows Kullan�c� Hesab� Crackleme

## Ni�in Kali?

- Kali se�memizin sebebi usb'den veya CD/DVD rom'dan live olarak yani kurulum yapmadan direkt �al��t�r�labilir olmas�d�r.
- Kali se�memizin bir di�er nedeni ise kullan�ca��m�z baz� haz�r paketlerin i�erisinde kurulu olarak gelmesi.

## Ad�m Ad�m Kullan�c� Hesab� Crackleme
- Kali linux'u boot etti�inizi ve kali linux masa�st�ne eri�ti�inizi varsay�yorum.
- �ncelikle disk yolunu ��renmeniz gerekiyor disk yolunu ��renebilmeniz i�in dosya y�neticisini a��p windowsun kurulu oldu�u dizinde bir dosyan�n �zerine sa� t�klay�n ve �zelliklere girin.
- "/root/493542/" benzeri yer alan ifadeyi alt taraftaki kodda **"DISKYOLU"** k�sm�na yerle�tirerek terminalde bu komutu �al��t�r�n.

![1. ad�m](images/windows-sifre/1.png)

```
cd /media/**DISKYOLU**/Windows/System32/config
````



- Geldi�imiz klas�rde windows'un kullan�c� hesab� bilgilerinin depoland��� .sam dosyalar� vard�r. Alt sat�rda verdi�im kodla bu dosyalar� g�rebilirsiniz.

![2. ad�m](images/windows-sifre/2.png)
```
ls -l SAM* sam*
```

- Bu g�rd���n�z sam dosyalar�n�n i�ini g�rme vaktimiz geldi.
![3. ad�m](images/windows-sifre/3.png)
```
chntpw -l SAM
```

- Ekranda g�rm�� oldu�unuz listede hesaplar ve hesaplar�n baz� �zellikleri yazmaktad�r. D�zenlemek istedi�iniz hesab� a�a��daki koda yerle�tirerek �al��t�r�n�z. Ben Camp kullan�c�s�n� se�tim.

![4. ad�m](images/windows-sifre/4.png)
```
chntpw -u **Administrator** SAM
```

- Gelen ekranda bize se�ti�imiz kullan�c� hesab�yla alakal� daha ayr�nt�l� bilgiler veriliyor.
- Bu ekranda 1,2,3,4,5 ve q komutlar�n� kullanarak baz� i�lemleri ger�ekle�tirebiliyoruz.

1- Kullan�c�n�n �ifresini kald�r
2- Kilidi kald�r ve hesab� aktif et(burada hesab�n aktif durumunu g�steriyor)
3- Hesab� y�kselt yani hesaba admin yetkilerini ver
4- Bir gruba kullan�c� hesab� ekle
5- Bir gruptan kullan�c� sil
q- ��k��

- Burdan diledi�iniz i�lemleri uygulad�ktan sonra q se�imini yaparak ��kabilirsiniz. "q" se�imini yapt�ktan sonra de�i�iklikleri onayl�yorsan�z "y" se�ip kaydediniz.
- Ard�ndan bilgisayar�n�z� yeniden ba�lat�p uygulad���n�z de�i�ikliklerin sonu�lar�n� alabilirsiniz.

