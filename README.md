## Merhaba!
> [!NOTE]
> Hurricane VR eklentisini kullanarak Unity üzerinden projesini geliştirmek isteyen kişilerin rahatlık ile sistemleri entegre edebilmesi için oluşturulmuş bir rehber. Eklenti geliştiricilerinin devamlılığı ve optimizasyon problemiyle karşılaşmamak adına Unity üzerinde her zaman lisanslı kullanımı benimseyiniz. (Harici sitelerden eklenen kaynak dosyaları her zaman sağlıklı bir şekilde çalışmayabilir, bundan dolayı resmi siteleri tercih edin.)

## İlgili Bağlantılar.
> [Eklentiyi Satın Al](https://assetstore.unity.com/packages/tools/physics/hurricane-vr-physics-interaction-toolkit-177300)

> [Unity İndir](https://unity.com)

> [Kod Düzenleyicisi İndir](https://code.visualstudio.com)

## Tıkla-Git.
- [Nesneler İle Etkileşim](https://github.com/thatsquecy/hurricane-vr-turkce-rehber/blob/main/README.md#nesneler-ile-etkileşim)
- [Nesnelerin Tutulması Sırasında Ellerin Pozisyonları](https://github.com/thatsquecy/hurricane-vr-turkce-rehber)
- [Nesnelerin Etkileşim Detayları](https://github.com/thatsquecy/hurricane-vr-turkce-rehber)
- [Tırmanma Mekaniği](https://github.com/thatsquecy/hurricane-vr-turkce-rehber)
- [Eşyalar İçin Yuva Sistemi](https://github.com/thatsquecy/hurricane-vr-turkce-rehber)
- [Kesici, Delici Aletlerin Saplanma Mekaniği](https://github.com/thatsquecy/hurricane-vr-turkce-rehber)

## Nesneler ile Etkileşim
Kullanıcı nesneler ile etkileşim haline geçmesi için belirli gereksinimlere ihtiyaç duyar, bu gereksinimler sırasıyla; etkileşime geçilecek nesnenin fizik kurallarına(RigidBody) ve içinden geçilmemesi adına bir yüzeysel sınıra(Collision) sahip olması, ek olarak VR sistemimizin onu algılayabilmesi için bir kod bütününe(Grabbable Scripti) ihtiyacı vardır. Oyuncunun aktif senaryo içerisinde kullandığı kumandalara ek bir el modeli vermek istenildiği durumlarda da kod bütünü dışında aynı gereksinimler bulunmaktadır. Bu bahsettiklerimizi nasıl sırasıyla basit şekilde ekleyeceğinizi aşağıya doğru indikçe rahatlıkla anlayacaksınız.

Öncelikle bir nesneyi nasıl fizik kurallarına entegre edeceğimizi ve yüzeysel sınıra sahip hale getirebileceğimizi inceleyelim. Unity'nin halihazırda sunmuş olduğu RigidBody ve Collider çeşitleri ile bu işleri halledeceğiz, örnek olarak farklı bir uygulama üzerinden oyunumuzda kullanacağımız modelinin çıktısını hazırladık ve Unity'e geçirdik. Unity'e geçmesinden itibaren model rahatlıkla kullanıcı gözünden görülebiliyor fakat herhangi bir şekilde fizik motorundan etkilenerek olduğu yerden kıpırdamıyor veya oyuncular bu nesnenin içerisinden geçebiliyorsa Rigidbody ve Collider eksikliğinden kaynaklıdır. Bu özellikleri nesnemize eklemek için Hierarchy penceresinden üzerine tıkladıktan sonra Inspector kısmından Add Component butonunu kullanıyoruz. Sırasıyla Rigidbody ve uygun Collider çeşitlerini nesnemize ekliyoruz.
**(Bu örneklendirmeler sıradan bir küp üzerinde yapılmıştır, rehberin ana amacı Hurricane VR eklentisi olduğundan dolayı Collision şekillendirmeleri ve Rigidbody detayları anlatılmayacaktır.)**


![image](https://github.com/thatsquecy/hurricane-vr-turkce-rehber/assets/48627621/a448f5a0-b810-4917-8c14-c4ec4e6bcd34)
![image](https://github.com/thatsquecy/hurricane-vr-turkce-rehber/assets/48627621/58cbab30-d280-464c-8bbd-c810b7efbcc1)
![image](https://github.com/thatsquecy/hurricane-vr-turkce-rehber/assets/48627621/116036e9-7da1-4780-aa3f-0a09a43e8e5d)

Rigidbody ve Collision eklentilerimizi ekledikten sonra Inspector penceresinde gelen eklenti kategorileri içerisinde nesnenin ağırlığı, yüzeysel sınırının çizgilerinin detaylı görünümü gibi özelliklere erişebilirsiniz.

![image](https://github.com/thatsquecy/hurricane-vr-turkce-rehber/assets/48627621/be307e78-7b77-41a6-9c9f-b9f1b2d89e8d)

Bütün bu işlemlerin ardından nesnemiz artık bir fiziğe sahip olacak, belirlediğiniz sınır yüzeyler kullanıcılar ve diğer nesnelerin ana nesnenin içinden geçmesini engelleyecektir. **(İç içe girmemesini istediğiniz bütün objelere Collision vermek zorundasınız, eğer ki diğer nesnelerin Collision'a sahip olmadığı sadece ana nesnenin Collision eklentisi barındırdığı durumda herhangi bir probleminiz çözülmeyecektir.)** Sırada Hurricane VR eklentisinin sunduğu Grabbable kod bütününü nesnemize uygulayarak onun kontrolcülerde atanan kavrama butonları aracılığıyla etkileşime geçebilir hale gelmesini sağlayacağız.

(...)

## Nesnelerin Tutulması Sırasında Ellerin Pozisyonları

(...)

## Nesnelerin Etkileşim Detayları

(...)

## Tırmanma Mekaniği

(...)

## Eşyalar İçin Yuva Sistemi

(...)

## Kesici, Delici Aletlerin Sağlanma Mekaniği

(...)
