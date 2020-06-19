# II Hafta (6-7 Haziran) Ödevleri 

## 6 Haziran Ödevleri:
- [ ] Github'ın Gitflow'u ile diğer yaklaşımları arasındaki fark nedir? ( gitflow vs ..)

 
 ##### [GitHub vs Gitlab](https://about.gitlab.com/devops-tools/github-vs-gitlab.html#recent-github-announcements)


##### GitHub vs Bitbucket

[https://www.elegantthemes.com/blog/wordpress/github-vs-bitbucket]: 

##### GitHub vs Azure Devops

- Azure DevOps nedir?
  Ekiplerin kod paylaşma, iş takibi ve yazılım gönderme hizmetleri. Azure DevOps, sınırsız özel Git barındırma, sürekli entegrasyon için bulut oluşturma, çevik planlama ve buluta ve şirkete sürekli teslimat için sürüm yönetimi sağlar. Geniş IDE desteği içerir.

- GitHub nedir? Açık kaynak ve özel geliştirme projeleri için güçlü işbirliği, inceleme ve kod yönetimi. GitHub, kodu arkadaşlarınızla, iş arkadaşlarınızla, sınıf arkadaşlarınızla ve yabancılarla paylaşabileceğiniz en iyi yerdir. Üç milyondan fazla insan birlikte harika şeyler oluşturmak için GitHub'ı kullanıyor.

  Azure DevOps "Proje Yönetimi" kategorisinde bir araç olarak sınıflandırılırken, GitHub "Kod İşbirliği ve Sürüm Kontrolü" altında gruplandırılabilir.

[https://stackshare.io/stackups/azure-devops-vs-github]: 

##### GitHub vs SVN

- SVN'nin ayrı bir sunucusu ve istemcisi vardır.

- Yalnızca bir geliştiricinin üzerinde çalıştığı dosyalar yerel makinede tutulur ve geliştiricinin sunucu ile çalışarak çevrimiçi olması gerekir. Kullanıcılar dosyaları teslim alır ve sunucuda değişiklik yapar.


[https://www.perforce.com/blog/vcs/git-vs-svn-what-difference]: 

##### GitHub vs Jira Software

[https://www.atlassian.com/software/jira/comparison/jira-vs-github]: 


 
  # GİTHUB BİRLEŞTİRME YÖNTEMLERİ ARASINDAKİ FARK

[https://rietta.com/blog/github-merge-types/]: 

### Create a Merge Commit

- Varsayılan seçenek Github'daki Çekme isteğini birleştirme seçeneği, tüm istekleri çekme isteğinden alır ve birleştirme işleminde yeni bir taahhütle ana şubeye ekler.
- Örneğin, ilk taahhüt ve 2 yeni taahhüt içeren bir ana master şubemiz var, yeni taahhütler Bir ve İki.

- Yeni bir özellik üzerinde çalışmak için ana daldan ayrılacağız ve özellik dalı adı verilen yeni bir dal oluşturacağız. Biraz iş yaptıktan sonra, ustayla birleştirmek istediğimiz Üç ve Dört tane 2 ek taahhüdümüz olacak.

- Birleştirme çekme isteği kullanılırken, (daha önce master'da hiçbir şeyin birleştirilmediği varsayılarak) 3 ve 4 taahhütleri ana şubeye birleştirme olarak eklenecek ve birleştirme dalı özellik-dalı olarak adlandıracağız. Bu yeni HEAD olacak.

- Depo geçmişini birleştir şube dalını birleştir. Git geçmişi Şubeyi birleştir özellik dalı gibi görünecektir. İleti tarafından sağlanan köprü, 3 ve 4 numaralı taahhütlerle orijinal PR'ye geri dönmenizi sağlar.

  ### Squash and Merge

- Squashing, bir şubeye yeniden basmak gibi çalışır, 5 taahhütlü çekme talebi alabilir ve tek bir taahhütte ezebilirsiniz. Bu, birleştirme çekme isteğine benzer görünebilir, ancak farklıdır.

- Geçmişte atılan commit’leri yeniden düzenlemek, isimlendirmek veya birleştirmek için kullanıyoruz.

  ### Rebase and Merge

  - Master a bir branch i rebase ettiğinizde , branch deki commitlerinizi tek tek alıp master ın sonuna ekleyecektir. Sonuç olarak rebase sonucunda tek bir history oluşturur çünkü tamamlanan işi bir branch ten diğerine aktarır. Bu süreçte istenmeyen history ortadan kalkar.
  - Merge yaptığmızda is yeni bir “ Merge commit” yaratıp iki branchinde tüm history(yapılmış tüm değişiklikleri) sini içerecektir. Master , branch te yapılan tüm değişiklikleri alacak ve entegre edecektir ancak branch in history sinde hiçbir değişiklik olmayacaktır.
  - Eğer tüm değişiklikleri görmek istiyorsanız merge yapmalısınız çünkü merge tüm değişiklikleri olduğu gibi korur.
  - Eğer daha sade, anlaşılabilir ve lineer bir commit history istiyor iseniz rebase sizin için daha yaralı olacaktır.
  - Eğer branchinizi push yaptıysanız merge, yapmadıysanız rebase i kullanmanız doğru olacaktır.

###       Merge Pull Request          

-   Bir çekme isteğini birleştirmeye hazır olduğunuzda ve hakemler onayladığında, çekme isteği      görünümünün sağ üst kısmındaki Birleştir'i tıklayın. Projede yazma (veya yönetici) izniniz varsa bir    çekme isteğini birleştirebilirsiniz.

  



[https://stackshare.io/stackups/azure-devops-vs-github]: 

# WHY GİT?

According to the latest [Stack Overflow developer survey](https://insights.stackoverflow.com/survey/2017#technology), more than 70 percent of developers use Git, making it the most-used VCS in the world. Git is commonly used for both open source and commercial software development, **with significant benefits** for individuals, teams and businesses.

- Stackowerflow anketine göre geliştiricilerin çoğunluğu GİT kullanıyor ve bu da GİT'i en çok kullanılar VCS yapıyor. Açık kaynak kodlu ve ticari geliştirmeler için çok yaygın kullanıma sahip.

- Geliştiricilerin herhangi bir projedeki değişikliklerin ,alınan kararların ve ilerlemelerin tüm zaman çizelgesini tek bir yerde görneylerini sağlar.
- DVCS ile kaynak bütünlüğü korunur.geliştiriciler güvenle üretim kodunda değişiklik önerebilir.

# ASP.NET Boilerplate-Web Application Framework

- Yazılım geliştirme görevlerini kurallara göre otomatik hale getirir.

- Projelerde **Authorization, Validation, Exception Handling, Logging, Localization, Database Connection Management, Setting Management, Audit Logging bunlardan bazıları. Ayrıca Katmanlı ve Modüler Mimari, Domain Driven Design, Dependency Injection** gibi katmanları best practice diyebileceğimiz mimari yapılar üzerine kurar, uygulama içerisindeki kodların belli bir mimariye göre benzer/ortak yapıda geliştirilmesi için çabalar.

- ```
  public class TaskAppService : ApplicationService, ITaskAppService
      {
          private readonly IRepository _taskRepository;
  
          public TaskAppService(IRepository taskRepository)
          {
              _taskRepository = taskRepository;
          }
  
          [AbpAuthorize(MyPermissions.UpdatingTasks)]
          public async Task UpdateTask(UpdateTaskInput input)
          {
              Logger.Info("Updating a task for input: " + input);
  
              var task = await _taskRepository.FirstOrDefaultAsync(input.TaskId);
              if (task == null)
              {
                  throw new UserFriendlyException(L("CouldNotFoundTheTask"));
              }
  
              input.MapTo(task);
          }
      }
  ```

Burada bir **Application Service** metodu görüyoruz. **DDD(Domain Driven Design)**’de Application Service’ler önyüzden direkt olarak kullanılan/çağırılan sınıflardır. UpdateTask metodunun AJAX ile çağırıldığını düşünebilirsiniz. Burada ASP.NET Boilerplate’in (kısaca ABP) bize ne sağladığına bakalım:

- **[Dependency Injection](http://www.aspnetboilerplate.com/Pages/Documents/Dependency-Injection)**: Bu (base class’dan dolayı) bir application service olduğu için Transient olarak Dependency Injection sistemine otomatik olarak kaydedilmiştir. Kendisi için gereken tüm servisleri (bu örnekte sadece bir Repository) direkt olarak inject edebilir (constructor ya da property injection yapılabilir). ABP conventional, kolay kullanımlı ve hazır bir DI altyapısı sağlar.

- [**Repository**](http://www.aspnetboilerplate.com/Pages/Documents/Repositories): Her Entity için otomatik olarak bir repository oluşturulur. IRepository<Task> şeklinde Task repository’sini kullanıyoruz burada. IRepository’nin birçok hazır metodu var. FirstOrDefault bunlardan birisi.

- [**Authorization**](http://www.aspnetboilerplate.com/Pages/Documents/Authorization): Eğer bu servisi çağıran kullanıcının “task güncelleme” yetkisi yoksa daha metod çağrısı başlamadan uygun bir authorization exception fırlatır. Attribute kullanarak authorization kontrolünü basitleştirmiş oluyoruz.

- [**Validation**](http://www.aspnetboilerplate.com/Pages/Documents/Authorization): UpdateTaskInput DTO’su (Data Transfer Object) içerisinde Task Entity’siyle isim ve tip olarak birebir eşleşen property’ler var. Normalde ilk iş bunların validate edilmesi gerekiyor. ABP data annotation’lar ve custom validation teknikleri kullanarak gelen input’un property’lerini otomatik olarak validate eder, eğer valid değilse client’ın anlayacağı formatta bir Exception fırlatır (AJAX çağrısı için uygun bir JSON döner örneğin). Ayrıca nesnenin kendisinin null olmasına da izin vermez, böylece input == null mı kontrolüne gerek kalmaz.

- [**Audit Logging**](http://www.aspnetboilerplate.com/Pages/Documents/Audit-Logging): Eğer audit logging açıksa bu metod çağrısını yapan kullanıcı, çağrının yapıldığı zaman, IP… gibi bilgilerle beraber çağrılan metod ve parametrelerini kaydeder. Ayrıca süre ölçümü de yapar, böylece yavaş metodlarımızı tespit edip kontrol edebiliriz.

- [**Unit Of Work**](http://www.aspnetboilerplate.com/Pages/Documents/Unit-Of-Work): Her application service metodu bir unit of work kabul edilir. ABP, metoda girerken veritabanı bağlantısını otomatik olarak açıp bir transaction başlatır. Eğer metod hiçbir Exception fırlatmadan başarıyla tamamlandıysa transaction otomatik olarak commit edilerek bağlantı kapatılır. Böylece metod içerisinde farklı repository’leri dahi kullansak tüm işlemler atomic olmuş olur. Ayrıca Entity’lerde yapılan tüm değişiklikler eğer hata olmazsa metod bitiminde otomatik olarak kaydedilir. Bu nedenle repository.Update(task) gibi bir kod çağrısına dahi gerek kalmamış oluyor.Burada birçok ayrıntı ve konfigurasyon var ancak varsayılan davranış bu şekildedir.

- [**Exception Handling**](http://www.aspnetboilerplate.com/Pages/Documents/Handling-Exceptions): Bir web uygulamasında, bu metod bir Exception fırlatırsa bu Exception otomatik olarak handle edilir, client’ın request türüne göre (AJAX ya da normal request) uygun bir dönüş değeri gönderilir client’a. Client tarafında da bu otomatik olarak handle edilerek kullanıcıya uygun hata mesajı gösterilir. UserFriendlyException özel bir exception türü olup direkt olarak mesaj kullanıcıya gösterilir. Diğer Exception’lar sadece loglanır ve kullanıcıya genel bir hata mesajı gösterilir.

- [**Logging**](http://www.aspnetboilerplate.com/Pages/Documents/Logging): UpdateTask metodunun ilk satırında direkt olarak hazır Logger nesnesini kullanarak log yazabiliyoruz. Varsayılan loglama kütüphanesi olarak Log4Net kullanılır.

- [**Localization**](http://www.aspnetboilerplate.com/Pages/Documents/Localization): Dikkat edilirse Exception fırlatılırken L adın bir metod kullanıldı. Bu da base class’dan gelen bir metod olup verilen key’e ve o anki kullanıcının diline göre ilgili lokalizasyon metnini verir.

- [**Auto Mapping**](http://www.aspnetboilerplate.com/Pages/Documents/Data-Transfer-Objects#DocAutoMapping): Son satırda ABP’nin MapTo extension metodunu görüyoruz. ABP, Automapper kullanarak bir nesneyi diğerine map edebilir. Böylece gelen input’daki (daha önce validate edilmiş) verilerle Entity’deki property’leri güvenle ezebiliyoruz.

- [**Dynamic Web API Layer**](http://www.aspnetboilerplate.com/Pages/Documents/Dynamic-Web-API): Bu application service aslında basit bir sınıftır. Browser’dan AJAX’la bunu çağırabilmek için genellikle wrapper şeklinde bir Web API Controller geliştirilir. ABP bu controller’ı runtime’da otomatik yaratır, böylece client’dan doğrudan application service’ler kullanılabilir olur.

- [**Javascript AJAX Proxy**](http://www.aspnetboilerplate.com/Pages/Documents/Dynamic-Web-API#DocDynamicProxy): Dinamik oluşturulan Web API’yi çağırmak için de ABP tarafından yine dinamik olarak bir javascript proxy’si oluşturulur. Böylece javascript’den metod çağırır gibi application service’leri kullanabiliriz.

  Görüldüğü gibi çok basit gözüken bu işlem için dahi bütün bunları manuel yapmaya kalsak oldukça zamanımızı alacakken ABP framework tüm bunları otomatik yaparak bizi benzer ve rutin işlemleri tekrar tekrar yapma zahmetinden kurtarır.



[http://devnot.com/2015/asp-net-boilerplate-modern-bir-web-uygulama-kutuphanesi/]: 

# RAZOR PAGES NEDİR?

- ASP.NET Core 2.0 ile hayatımıza girdi.ASP.NET Core MVC alt yapısında sayfa bazlı web uygulama geliştirebileceğimizprogramlama modelidir.

- MVC template'lerindeki klasör sayısını azaltmak ,sayfa bazlı uygulamaları kolayca geliştirmek için tasarlanmış bir model.
 
[https://www.minepla.net/2017/09/asp-net-core-razor-pages-nedir/]: 





[https://www.perforce.com/blog/vcs/git-vs-svn-what-difference]: 

##### GitHub vs Jira Softwar

[https://www.atlassian.com/software/jira/comparison/jira-vs-github]: 

- [ ] [Git and GitHub with Briana Swift](https://www.youtube.com/playlist?list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4) Youtube Listesi incelensin. (11 Video)
- [ ] Merge pull request
    - [ ] Create a merge commit
    - [ ] Squash and merge 
    - [ ] Rebase and merge altında ne fark var (Ödev)
- [ ] issue ve #pull request de id ler neden artıyor farklı sekmeler olmasına rağmen?
- [ ] [Ramp up on Git and GitHub](https://lab.github.com/githubtraining/paths/ramp-up-on-git-and-github) (ödev)
- [ ] Aspnetboilerplate ve yan ürünler araştırması. [AspNet Boilerplate - Web Application Framework](https://aspnetboilerplate.com/)
- [ ] hackerRank.com --> [30 Days Of Code](https://www.hackerrank.com/domains/tutorials/30-days-of-code)

## 7 Haziran Ödevleri:
- [ ] Razor Pages Nedir?
- [ ] 4 Farklı Projede Yapılacak *Change Authentication* :
  - [ ] No Authentication
  - [ ] Individual User Account
  - [ ] Work or School Accounts
  - [ ] Windows Authentication seçili projeler oluşturulmalı
- [ ] Ayarlardaki Output kısmındaki Console Application nedir? diğerleri arasında fark nedir? [Ders Akışındaki 6. Madde'yi inceleyin.] ( araştırma ödev verildi ).
- [ ] c# json serialize / deserialize
- [ ] MVC vs MVVM
   - [ ] MVP vs MVW vs MVU Pattern arasındaki farkı araştır
   - [ ] Model-View-Update (MVU) nedir?
