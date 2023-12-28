---
title: "YAZILIM SEKTÖRÜNDE İŞ VE ÖZEL HAYAT DENGESİ"
date: 2021-09-27T15:00:04+02:00
draft: false
---

Geçen hafta, yazılım geliştiriciliğin rahat olduğunu söylediğim [şu tweet](https://twitter.com/omurturan/status/1440346021108666384) yüzünden ufak çaplı bir linç yedim. Fikir ayrılıkları hiç problem değil ama işin bir noktadan sonra hakaret boyutuna varması bir miktar moralimi bozdu. Neyse ki sosyal medyada her şey 24 saat içinde unutuluyor. Gelen tepkilerden anlaşıldığı üzere bu meslek herkes için aynı zorluk seviyesinde değil. Kendi zorlandığım noktalarda uyguladığım birkaç tekniği paylaşmak istedim

Bu yazıda tweete yanır olarak gelen şu argumanlara değineceğim:
- Öğrenmesi hiç bitmiyor
- Sabaha kadar kod yazıyorum
- Beynimde sürekli iş ile ilgili sorunlarla uğraşıyorum
- Yazılım yüzünden belim ağrıyor
- Yazılım yüzünden saçım döküldü
- Yazılıma rahat dediğiniz için mesleğe saygı kalmadı 😞
- Bu dediklerin iyi güzel ama bizim şirkette çalışmaz

## Öğrenmesi hiç bitmiyor

Gelen yanıtlarda en çok bahsi geçen ve benim de en çok katıldığım zorluk, bu mesleğin gerçekten hiç bitmeyen bir öğrenme süreci içermesi. Şu anda kullandığınız populer bir framework, 2 yıla piyasadan silinmiş olabiliyor. Şu anda kullandığınız bir dil, birkaç yıl içinde yeni versiyonları çıkmış ve sizi tamamen yabancı durumuna düşürmüş olabiliyor. Peki bununla başetmenin yolu nedir?

Günlük hayattaki işlerin peşinden koşarken durup kendini bir konuda geliştirecek vakit bulmak çok zor olabiliyor. Haftasonu geldiğinde yine "iş" ile ilgilenmek, mental sağlığımız açısından çok iyi bir yöntem olmayabilir. Ee peki ne zaman yeni teknolojileri öğreneceğiz? Günümüzde bir sürü şirkette/ekipte uygulandığını gördüğüm bir yöntem var: teknik konuları ekipçe öğrenmek. Bu şekilde bu öğrenmeye mesai saatleri içinde bir vakit ayırmak mümkün. VueJS v2 kullanan bir takım hep beraber oturup v3'te neler varmış diye kendi içinde yarım günlük bir etkinlik yapsa, çoğu şirketin buna laf edeceğini sanmıyorum.

Bu işin bir de maddi boyutu var tabii ki. Ekonomik durumunuza göre sırf bu konu bile üstünüzde bir gerginlik yaratıyor olabilir. Okumanız gereken teknik kitaplar, eğitimler, konferansların bir çoğu ücretli. Yine günümüzde çoğu şirkette kişisel gelişim bütçesi var. Az veya çok olsa da böyle bir bütçe, üzerinizdeki yük bir miktar hafifletebilir. Çalıştığınız şirkette böyle bir bütçe yoksa talep ediniz. Çok olsa hayır derler. 😄

## Sabaha kadar kod yazıyorum

Öncelikle bunun adı fazla mesaidir. Fazla mesaiyi yazılım sektörünün bir parçası sanan birçok meslektaşım olduğunu görmek biraz üzücü oldu. Sabaha kadar kod yazmak, filmlerde gösterildiğinin aksine, "cool" bir durum değil. Fazla mesai nerede olursa olsun yıpratır. Örneğin, benim kontratımda haftalık 40 saat çalışacağım yazıyor. Teorik olarak bundaz fazla çalışmamam lazım. Günlük hayatta ise bu pek böyle olmuyor tabii ki. Peki yazılım sektöründe en çok hangi durumlarda fazla mesai yapıyoruz ve bundan nasıl sağ çıkabiliriz?

Herhalde fazla mesai beklenen en tipik durum, bitmesi gereken gecikmiş bir proje olması. Bu çok anlaşılabilir bir durum. Hayatta her şey planladığımız gibi gitmez. Fakat bazı firmalarda bunun artık olağan bir hale gelmiş ve kurum kültürüne işlemiş olduğunu görüyorum/duyuyorum. Çok sayılmaz ama ben yaklaşık 10 senedir bu meslekten para kazanıyorum. Şimdiye kadar görmüş olduğum kadarıyla, acil denen, bitmezse ölürüz biteriz denen projelerin %90'ının acil olmadığı. Bence yapılan her fazla mesaiden sonra, bunu bir başarısızlık kabul edip, bir daha olmaması için bir tur sorgulama yapılması gerekiyor. Bu yapılmazsa, proje yönetimi açısından her şey çok sağlıklı görüneceği için bir sonraki planlamalar da yine aynı şekilde yapılacak ve fazla mesai sonraki projelerde de kaçınılmaz olacaktır.

Fazla mesaiden sonra yapılması gerekenler:
- Bir daha yaşanmaması için yapılması gereken planlama değişiklikleri
- Fazla mesainin telafi edilmesi (izin, para, bonus vs.)

Sabaha kadar çalışılan bir diğer durum da heralde üründe çok ciddi bir hata olması durumlarında yaşanıyor. Bu gibi durumlara doğal afet gözüyle bakmak lazım. Olduğu anda çoğu zaman elinizde çok kısıtlı seçeneğiniz olur. Bunlara önceden hazırlanmak gerekiyor. Örneğin, deployment için kullandığınız aracın, uygulamanın eski versiyonlarına dönmeyi çok kolay hale getirmesi gerekiyor. Eğer gündüz, içinde bug bulunduran bir kod deploy edilmişse ve siz gece 2'de bununla ilgili uyarı alıyorsanız, bir tık ile uygulamayı eski versiyonuna döndürebilmeli ve sonra uykunuza geri dönebilmelisiniz. Bug'ı çözmek yarının görevi. Bu bir teknik makale değil. O sebeple ayrıntıya girmeye daha fazla gerek yok sanırım ama gerçek hayatta olduğu gibi, doğal afetlere geniş zamanda hazırlanmak lazım. Hazırlanırken de benim aklımda hep aynı soru oluyor genelde: Gece 2'de bir sorundan dolayı uyanırsam, uykuma en çabuk nasıl dönerim? Monitoring araçlarınız, oncall sisteminiz, hangi metrikleri takip ettiğiniz, rollback mekanizmaları vs gibi konuları önceden düşünürseniz gece uyandığınızda çok daha az stresli geçecektir.

## Sabaha kadar beynimde iş ile ilgili sorunlarla uğraşıyorum

Mesai bitince zihnimizi sıfırlamak her zaman mümkün olmayabiliyor. Bu konuda bana faydalı olan birkaç yöntem var. Bir tanesi meditasyon. Headspace uygulaması ile guided meditation yapmaya başladım. Gün ortasında veya sonunda, ne zaman stresli hissedersem 7-10 dakika arası bir meditasyon seansı bir miktar zihnimi boşaltmamı sağlıyor. Meditasyon çok havalı bir kelime gibi duruyor da mesela bulaşıkları elde yıkıyorsanız o da aynı görevi görebilir. 😄 Burada önemli nokta zihnimizi iş düşünmekten alıkoyacak bir aktivite yapmak. Meditasyon bana göre değil diyorsanız, işten sonra herhangi bir hobinizle ilgilenmek, (mümkünse iş dışı) arkadaşınızla kahve içmeye çıkmak, özellikle spor yapmak bana iyi gelen şeyler.

Diğer yöntem ise, çalıştığım yer ile yaşadığım yeri mümkün mertebe ayırmaya çalışmak. Benim ayrı bir çalışma odam maalesef yok ama evdeki bir köşeyi çalışma köşem yaptım. Oraya sadece çalışmak için gidiyorum. Çalışmam bitince oraya gitmemeye çalışıyorum. Bu aralar da zorunlu olmamasına rağmen ofise çalışmaya gidiyorum. Mesai bitince laptopun kapağını kapatıp binayı arkamda bırakıp çıkıp gitme hissi çok güzel.

Bunun yanında sanal izolasyon da çok önemli. İş ve özel işlerimiz için farklı tarayıcılar kullanmak, mesai dışında bildirimleri sınırlamak veya kapatmak, haftasonları veya tatillerde iş maillerine bakmamak gibi yöntemleri kullanıyorum. Birçoğumuz sabah kalkar kalkmaz telefona bakıyoruz muhtemelen. Sabah kalkınca Twitter'a bakmak ile iş maillerine bakmak arasında fark var.Maillerimize bakınca, zihnimizde artık iş başlamış oluyor ve sonra kahvaltı yapsak bile zihnimiz iş düşünmeye başlıyor. Bunların hepsi herkes için uygulanabilir olmayabilir tabii ki ama eminim sizin için daha iyi olacak sınırlar belirleyebilirsiniz. Siz kendiniz için sınırlar koymazsanız, bir başkası bunun sizin adınıza yapmaz.

## Yazılım yüzünden belim ağrıyor

Ben de bu hatayı çok uzun süre ve ısrarla sürdürdüm. Siz yapmayın ve vakit kaybetmeden düzgün bir masa ve sandalye alın. En pahalı sandalye en iyi sandalye demek değil ama iyi sandalyeler maalesef pahalı. Vücut ölçülerinize da dikkat ederek bir masa sandalye edinin mutlaka.

Bizim gibi bütün gün oturarak işini yapan insanlar olarak sporu da bir şekilde hayatımıza dahil etmek gerekiyor. Bu yazıyı 20'li yaşlarında okuyup benim belim ağrımıyor ki diye düşünen varsa bu hatadan vazgeçsin.


## Yazılım yüzünden saçım döküldü

Yazılımdan değildir o, dayın keldir. 😄 Şaka bir yana stres önemli bir faktör. Stresle başetmek için sihirli bir formülüm yok maalesef.

## Yazılıma rahat dediğiniz için mesleğe saygı kalmadı 😞

Evet ben tweet attıktan sonra bizim şirket de bunu farketti ve yazılım departmanının maaşlarını %10 düşürdü. Yazılımın ne kadar zor olduğu ile ilgili başka bir tweet üzerinde çalışıyorum. 😞

## Bu dediklerin iyi güzel ama bizim şirkette çalışmaz

Haklısın ama biz sormadığımız için olmuyor. Öyle değilmişiz gibi davranan meslektaşlarım var ama biz işçiyiz. Biz istemeden kimse bize ekstra hak vermez. Şu anda şanslıyız ki yazılım çok işçi açığı olan bir sektör. O sebeple elimiz biraz daha kuvvetli. Genelde bulunduğunuz şirketi bir lafla değiştirmek zor. Çoğu şirkette bu değişim çalışacak eleman bulamadığı zaman oluyor.

Hiçbir şirket mükemmel değil ama bazıları diğerlerinden daha adil davranıyor. Size daha adil davranan şirketlerde çalışın.
