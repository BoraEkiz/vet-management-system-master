
## Özellikler

- Müşterileri kaydetme, güncelleme, görüntüleme ve silme
- Hayvanları kaydetme, güncelleme, görüntüleme ve silme
- Hayvan sahiplerini ve hayvanları isme göre filtreleme
- Hayvanlara uygulanan aşıları kaydetme, güncelleme, görüntüleme ve silme
- Hayvan sahiplerine ait hayvanların görüntülenmesi
- Randevu oluşturma, güncelleme, görüntüleme ve silme
- Doktorların müsait günlerini yönetme

##  Kurulum

2. Gerekli bağımlılıkları yükleyin:
    ```sh
    ./mvnw clean install
    ```

3. Veritabanını yapılandırın (aşağıdaki Veritabanı Ayarları bölümüne bakın).

## Çalıştırma

Uygulamayı aşağıdaki komutla başlatabilirsiniz:
```sh
./mvnw spring-boot:run
```

## Veritabanı Ayarları

Veritabanı Ayarları
Uygulama, PostgreSQL veritabanı kullanmaktadır. application.properties dosyasındaki ayarları aşağıdaki gibi yapılandırın:

```
spring.application.name=Vms
spring.jpa.show-sql=true
spring.jpa.hibernate.ddl-auto=create-drop
spring.datasource.url=jdbc:postgresql://localhost:5432/VeterinaryBase
spring.datasource.username=postgres
spring.datasource.password=postgres
spring.datasource.driver-class-name=org.postgresql.Driver
spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect
```


