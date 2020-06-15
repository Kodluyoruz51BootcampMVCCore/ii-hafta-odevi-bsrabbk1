# II Hafta (6-7 Haziran) Ödevleri 

## 6 Haziran Ödevleri:
- [ ] Github'ın Gitflow'u ile diğer yaklaşımları arasındaki fark nedir? ( gitflow vs ..)

 
 ##### GitHub vs Gitlab

![](C:\Users\bebek\OneDrive\Masaüstü\github_comparison.png)



[https://about.gitlab.com/devops-tools/github-vs-gitlab.html#recent-github-announcements]: 

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



![]()![DfD6muTWAAE-Ei7](C:\Users\bebek\OneDrive\Masaüstü\DfD6muTWAAE-Ei7.jpg)
 
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





[https://www.perforce.com/blog/vcs/git-vs-svn-what-difference]: 

##### GitHub vs Jira Software

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
