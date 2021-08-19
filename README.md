# DevOpsSinav2
Bu repository docker-compose ile elastichsearch ve kibana kurulumlarını, ansible ile yazdığımız docker-compose ve metricbet, filebeat kurulumlarını içermektedir.

1-Elasticsearch, Kibana uygulamalarını docker compose ile çalıştırın

Docker-compose birden fazla containerlarımız oluşturmak için kullanıyoruz.

<img width="627" alt="Screenshot 2021-08-19 at 16 18 51" src="https://user-images.githubusercontent.com/82338626/130075507-db3163fd-7087-4922-883e-a0cc6ab7bec3.png">

docker-compose up -d lomutu ile oluşturduğumuz docker-compose dosyasını çalıştırıyoruz.

docker ps komutu ile containerlarımızın ayağa kalktığını görebiliyoruz.

<img width="1538" alt="Screenshot 2021-08-19 at 16 20 17" src="https://user-images.githubusercontent.com/82338626/130075785-b94ec0c2-23b3-4a9c-ba87-fceed2abd610.png">

sonrasında browser üzerinde elasticsearch ve kibana arayüzlerine erişiyoruz.

ElasticSearch: Dış uygulamalar üzerinden toplanan verilerin analizi ve içerik arama gibi işlemleri yapmamızı sağlayan bir search Engine(Arama Motoru) dir.

Logstash: Toplanan verilerin düzenlenip, anlamlı hale gelebilmesini sağlayan araçtır.

Kibana: Toplanıp anlamlı hale gelen verinin, analizini yaptıktan sonra ki görselleştirme işlemini yapar.



Sonraında Filebeat ve metricbeat kurulumlarını manuel olarak gerçekleştirip her biri için elastichsearch ile configurasyonlarını yapıp kibana üzerinde izlemek istediğim logların geldiğini gördüm.

Filebeat; clientlar üzerinde agent rolü ile loglarınızı forward etmenize yarayan bir yazılımdır, tek amacı loglarınızı hedeflediğiniz yere değişimsiz taşınmasıdır.

Metricbeat ElasticSearch ‘ün  pluginlerinden birisidir. Metricbeat   ile işletim sisteminden ve sunucu da çalışan servislerden düzenli aralıklarla kullanılan modüllere göre verileri toplayarak elasticsearch de  bu verileri tutan ve içerisinde bulunan dashboardlar ile sistem ve servisleri izlememize olanak sağlayan plugindir.

<img width="1041" alt="Screenshot 2021-08-19 at 16 27 23" src="https://user-images.githubusercontent.com/82338626/130076788-fc568c05-ff91-491b-8450-438b0280bd12.png">



Son adımda da kibana arayüzünde izlediğimiz verilerin görselleştirmesini yaptım.

