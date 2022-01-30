# AppJar Yardım Dökümanı

## AppJar paketinin kurulumu

Ayarlar sekmesi altındaki kutu ikonuna tıklayarak Paket Yöneticisi açılır.

![139532096-74f54990-8b87-41ad-88c6-9a36899318d1](https://user-images.githubusercontent.com/56628866/142197857-48387968-c820-4a09-9fb0-31f61e9179e6.png)

Paket yöneticisine tıklandığında karşınıza kurulu paketleri görebildiğiniz veya yeni paketler kurabildiğiniz bir pencere çıkar.

![image](https://user-images.githubusercontent.com/56628866/142198242-40f9a83c-dcd9-4e50-8746-9fa280286697.png)

Arama kutusuna AppJar yazıp PyPl'dan Paket Bul butonuna tıklayın.

![image](https://user-images.githubusercontent.com/56628866/142198522-ebc65d4f-e3c0-4b03-a9cb-a6b2f44e17dd.png)

Paket bulunduğunda pencerenin sağ tarafında paketle ilgili bilgileri ve kur butonunu görebilirsiniz.

![image](https://user-images.githubusercontent.com/56628866/142198618-ff8d857b-7265-4552-8c41-d8b024793270.png)

Kur butonuna tıkladığınızda kurulum başlayacaktır. Kurulum bitene kadar bir süre bekleyiniz.

![image](https://user-images.githubusercontent.com/56628866/142198726-ae9276cb-95c8-4ed8-90b2-cb7f2290b088.png)

Kurulum bittiğinde İndirme başarılı yazan bir pencere çıkacaktır.

![image](https://user-images.githubusercontent.com/56628866/142198802-089a2694-700e-4771-b681-c9475c019f9f.png)

Paket Kullanıma hazır.

## Pencere

### Pencere Oluşturma

Pencere oluşturmak için AppJar kütüphanesinden gui (Görsel kullanıcı arayüzü) sınıfının içe aktarılması gerek. **p = gui()** yazarak p adında bir pencere oluşturabiliriz. gui() sınıfına ait **go()** metodu ise oluşturulan pencereyi başlatır.

**Örnek**

```python
#appJar kütüphanesinden gui sınıfını içe aktar
from appJar import gui 

#Sonra pencere objesini oluştur
p = gui()

#Son olarak pencereyi başlat
p.go()
```

![image](https://user-images.githubusercontent.com/56628866/151692123-4df5584a-2d42-40de-bb82-e63f15117aac.png)


### Pencere Boyutu

Oluşturulan bir pencerenin boyutunu ayarlamak için gui() sınıfına ait **setSize()** metodu kullanılır. parametre olarak ilk önce pencerenin eni sonra da boyu aralarına virgül(,) konarak girilir.

**Örnek**

```python
from appJar import gui 
p = gui()

#Pencerenin en,boy uzunluklarını 300,200 olarak ayarla
p.setSize(300,200)

p.go()
```

![image](https://user-images.githubusercontent.com/56628866/151692152-3b83cb37-ca59-4d2d-9521-964c72d3929a.png)

### Pencere Başlığı

Oluşturulan bir pencerenin başlığını ayarlamak için gui() sınıfına ait **setTitle()** metodu kullanılır.

**Örnek**

```python
from appJar import gui 
p = gui()
p.setSize(300,200)

#Pencerenin başlığını 'Başlık' olarak değiştir
p.setTitle("Başlık")

p.go()
```

![image](https://user-images.githubusercontent.com/56628866/151692212-aaca8552-74fc-459e-bd4f-4865211e023b.png)

### Pencere Arkaplan Rengi

Oluşturulan bir pencerenin Arkaplan rengini ayarlamak için gui() sınıfına ait **setBg()** metodu kullanılır. Parametre olarak temel renklerin isimleri ingilizce olarak girilir.

**Örnek**

```python
from appJar import gui 
p = gui()
p.setSize(300,200)

#Pencerenin arka plan rengini yeşil yap
p.setBg('green')

p.go()
```

![image](https://user-images.githubusercontent.com/56628866/151692270-afeb612c-888a-4261-bbee-ead08ce4b3a0.png)





































