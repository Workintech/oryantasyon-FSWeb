# Git Konfigurasyonu

Bu github repository, Git ve GitHub hesaplarınızın kurulumunda size yol gösterecektir. Bu projenin amacı, bilgisayarınızın ortamının doğru şekilde ayarlandığından emin olmak ve Git iş akışının bir önizlemesini oluşturmaktır. Her komutun ek işlevselliği ve açıklamaları ile Git'e daha derinlemesine bir giriş, WorkinTech’te devam eden öğreniminizin bir parçası olacaktır.

---

## Adımlar

- [x]  README’yi görüntüleme
- [x]  Bir GitHub hesabı oluşturma
- [x]  Komut satırı arayüzünü açma
- [x]  Kullanıcı Adı and E-mail oluşturma
- [x]  Kimlik doğrulamasının yapılması
- [x]  Repository’nin forklanması 
- [x]  Repository’nin clone’lanması
- [x]  Repository’de değişiklik yapma
- [x]  Değişiklikleri Local olarak commit etmek
- [x]  Değişiklikleri GitHub'a Taşıma
- [x]  Standart İş Akışı


---

## README’yi görüntüle
İlk adım tamamlandı. Hoş geldiniz ve sonraki adımlarda iyi şanslar.
Sorunlarla karşılaşırsanız lütfen Hub'ın tartışma forumlarını ziyaret edin veya yardım için bize başvurun.

---

## GitHub Hesabı Aç
*Sadece bir kez.*

Henüz bir GitHub hesabı oluşturmadıysanız, bu [GitHub](https://github.com/) bağlantısını izleyin.
> Kaydol'a tıklayın ve talimatları izleyin. 
> Kurulum sırasında muhtemelen son adım olan e-postanızı doğrulamanız gerekecektir.

---

## Komut Ekranını Aç 
*Kariyerinizde sık sık kullanacağınız için bu adıma aşina olun.*

MacOS
> Terminal'i açın: `Command Key + Spacebar` ardından aramaya `terminal` yazın.

Windows
> Henüz yapmadıysanız Windows için [GitBash](https://git-scm.com/downloads)'i yükleyin.  
> GitBash'i açın: `Windows Key` ve ardından arama kısmına `git bash` yazın.

---

## Kullanıcı Adı ve E-mail Oluşturma
*Bu adımın kullanacağınız her farklı bilgisayar için bir kez tamamlanması gerekecektir.*

1. Komut satırı arayüzünüzde şunu yazın: 
    ```
    git config --global user.name "Put your Name in Here"
    ```
    ```
    git config --global user.email your@email.here
    ```

2. İşe yarayıp yaramadığını kontrol edin. 
    ```
    git config --list
    ```
    yazın.

    Bu listede value’larınızla eşleşen iki satır görmelisiniz. Listede başka satırlar da olabilir.
    ```
    user.name=Deniz Acay
    user.email=deniz@workintech.com.tr
    ```
---
    
## Kimlik Doğrulamasının Yapılması
*Bu adımın kullanacağınız her farklı bilgisayar için bir kez tamamlanması gerekecektir.*
  
SSH kurulumu için bir video ile birlikte hareket etmeyi veya talimatları doğrudan GitHub'dan takip etmeyi seçin.
> [Windows Video Anlatım](https://cdn.journeyapp.com/contents/wIdI3h0bwrFR2Lj7e8bqkTa8lz8Hu5PnTHQY6uH1AblukwLP0O7VxnTnnToY6Giu_1666349118.mp4)  
> [GitHub Adımları](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) (Uygun işletim sistemini seçtiğinizden emin olun.)

---

## Repository’nin Forklanması
*Bu adımın GitHub'da kendi kopyanıza sahip olmak istediğiniz her repository için bir kez tamamlanması gerekecektir.*
1. Bu README'nin bulunduğu GitHub sayfasında, sağ üst tarafa yakın bir yerde `Fork`'u seçin.
2. `Owner` altında accountunuzu seçin.
3. `Repository name` adı altında, isterseniz repository’nizin adını değiştirebilirsiniz.
4. Sayfanın alt kısmında `Create fork`'u seçin.
5. GitHub'daki user account’ınızla ilişkili yeni bir repository’e yönlendirilmeniz gerekir.

---

## Repository’nin Clone’lanması
*Bu adımın kendi bilgisayarınıza yerleştirmek istediğiniz her repository için bir kez yapılması gerekecektir.*

1. GitHub'da yeşil `Code` düğmesini bulun ve seçin.
2. Şu anda seçili değilse `SSH`'yi seçin.
3. Görüntülenen `git@github.com:...` linkinin yanındaki `copy` simgesini seçin.
4. Komut Satırı Arayüzünüzde, bu repository’i saklayacağınız directory’e(dizin) geçerek başlayın. 
    Örnek: `cd ~/Workintech-Repos/`  
    Yeni bir dizin oluşturmanız gerekiyorsa aşağıdaki adımları izleyin:
    ``` 
    cd ~
    mkdir Workintech-Repos
    cd Workintech-Repos
    ```
5. `git clone` yazın sonra sağa tıklayın ve kopyaladığınız metni yapıştırın.
    > Örnek:`git clone git@github.com:kullaniciadiniz/oryantasyon-git.git`
6. Kendi bilgisayarınızda yeni klonlanmış repository'i görüntülemek için `ls` yazın.

---

## Repository’de Değişiklik Yapma
*Bu adım genellikle projeniz üzerinde entegre geliştirme ortamları ile çalışmanızı içerecektir*
1. CLI'nızda `cd bd-orientation` yazarak klonladığınız repository’e gidin. Dizin adınız biraz farklı olabilir.
2. `ls` yazın . README.md adlı bir dosya görmelisiniz.
3. Bir sonraki hedefiniz bu dosyayı açmak ve düzenlemektir. Aşağıdaki talimatlar basic text editor kullanacaktır, ancak dosyayı içindeki text’i değiştirmek için istediğiniz şekilde açabilirsiniz. 
    > MacOS: `open -e README.md` yazın
    > Windows: `notepad README.md` yazın
4. Checklist’te tamamladığınız her adıma bir `x` işareti koyun. Bu, bir proje üzerinde çalışırken dosyaları değiştirmenizi simüle eder.
   ‘Değişiklikleri Local Olarak İşleme’ veya ‘Değişiklikleri GitHub'a Taşıma’ bölümlerine henüz bir `x`işareti koymamalısınız.
4. Değişiklikleri kaydedin/
    > MacOS: `Command S`'e basın.
    > Windows: `CTRL S`'e basın.
6. Editor’ünüzü kapatın ve komut satırı arayüzüne dönün. Hala daha önce bulunduğunuz dizinde olmalısınız.

---

## Değişiklikleri Local Olarak Commit Etmek
*Bu adım genellikle bir projede bir veya daha fazla kez yapılacaktır. Daha büyük projeler bu adımı birçok kez tamamlamanızı gerektirebilir.*
1. Komut satırınıza şunu yazın: 
    ```
    git add .
    ```  
    Dikkat: Yukarıdaki `.` kasıtlıdır. Bu `.` Git'te değiştirilen tüm dosyaları eklemesi için tanımlar.
2. 
    ```
    git commit -m "Checked off my finished tasks"
    ```
    yazın.

    Dikkat: Yukarıdaki mesajdaki `"`tırnak işaretlerine`"` dikkat edin. Tırnak işaretlerini başlattığınızdan ve sonlandırdığınızdan emin olun.

---

## Değişiklikleri GitHub'a Push Etme
*Bu adım genellikle bir projede bir veya daha fazla kez yapılacaktır. Codegrade'e bağlıysanız, bu işlem projenizin yeniden puanlanmasına neden olacaktır.*
1. 
    ```
    git push
    ```
    yazın.
2. GitHub repository sayfanıza dönün. Gerekirse  bir refresh yapın.
3. README.md dosyasının yakın zamanda güncellenip güncellenmediğini kontrol edin.
4. Bitirdiğiniz `x`'leri görmek için aşağı kaydırın.

---

## Standart İş Akışı ##
1. Local computer’da,  README.md dosyasını tekrar düzenleyerek `x`'i artık tamamlanmış görevlerinize ekleyin.
   > Teknik olarak Standart İş Akışı görevini bitirmediniz, `x` işareti olmadan bırakın.
2. Ekleme, commit etme ve push etme alıştırmaları yapın. Güncellemelerinizin GitHub'da görünüp görünmediğini kontrol edin.
   > Mesajı buna göre düzenleyin, örnek:  `Checked off additional finished tasks`
3. Son `x`’iniz için bu işlemi son bir kez tekrarlayın. Sürece aşina olmanıza yardımcı olur.

---

## Tebrikler!! ##
Git, muhtemelen kariyeriniz boyunca her gün kullanacağınız bir araç olacaktır.

Bu, bilgisayarınızın ortamının doğru ayarlandığından emin olmak için Git'e minimal bir girişti. Ek işlevsellik ve açıklamalarla Git'e daha derin bir giriş, Workintech'te devam eden öğreniminizin bir parçası olacaktır.
