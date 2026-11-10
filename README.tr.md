<a id="readme-top"></a>

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![Tampermonkey][tampermonkey-shield]][tampermonkey-url]

<br />
<div align="center">
  <h3 align="center">Reddit Unfollow All</h3>

  <p align="center">
    Reddit alt dizin aboneliklerinden toplu olarak çıkmanızı sağlayan, sürüklenebilir kontrol paneline ve ayarlanabilir hıza sahip bir kullanıcı betiği.
    <br />
    <a href="https://github.com/aybrkaknc/RedditUnfollowAllScript"><strong>Depoyu keşfedin</strong></a>
    <br />
    <br />
    <a href="https://github.com/aybrkaknc/RedditUnfollowAllScript/issues/new?labels=bug">Hata Bildir</a>
    &middot;
    <a href="https://github.com/aybrkaknc/RedditUnfollowAllScript/issues/new?labels=enhancement">Özellik İste</a>
  </p>

  <p align="center">
    <a href="README.md">English</a> | <a href="README.tr.md">Türkçe</a>
  </p>
</div>

<details>
  <summary>İçindekiler</summary>
  <ol>
    <li>
      <a href="#proje-hakkında">Proje Hakkında</a>
      <ul>
        <li><a href="#kullanılan-teknolojiler">Kullanılan Teknolojiler</a></li>
      </ul>
    </li>
    <li>
      <a href="#başlarken">Başlarken</a>
      <ul>
        <li><a href="#gereksinimler">Gereksinimler</a></li>
        <li><a href="#kurulum">Kurulum</a></li>
      </ul>
    </li>
    <li><a href="#kullanım">Kullanım</a></li>
    <li><a href="#teknik-notlar">Teknik Notlar</a></li>
    <li><a href="#katkıda-bulunma">Katkıda Bulunma</a></li>
    <li><a href="#iletişim">İletişim</a></li>
    <li><a href="#teşekkürler">Teşekkürler</a></li>
  </ol>
</details>

## Proje Hakkında

Reddit Unfollow All, Reddit alt dizin aboneliklerinden çıkma işlemini otomatize eder. Alt dizin listesi sayfasına müdahaleci olmayan bir arayüz ekler ve çıkma işlemlerini tek tek çalıştırır. Hız hazır ayarları, platformun hız limitlerine takılmanızı önlemeye yardımcı olur.

- **UI Katmanı**: Küçültme ve kapatma kontrolleriyle sürüklenebilir panel.
- **Throttling (Hız Sınırı)**: 200ms ile 1500ms arasında hazır çalışma aralıkları.
- **Durum Takibi**: Panel üzerinde toplam ve kalan işlem sayısı ile işlem günlüğü.
- **Dil Desteği (i18n)**: Tarayıcı dilini otomatik algılar (Türkçe ve İngilizce).
- **DOM Uyumluluğu**: Eski (`old.reddit.com`) ve modern Reddit arayüzleri için seçici desteği.

<p align="right">(<a href="#readme-top">başa dön</a>)</p>

### Kullanılan Teknolojiler

* [![JavaScript][JavaScript-shield]][JavaScript-url]
* [![Tampermonkey][Tampermonkey-badge]][Tampermonkey-url]

<p align="right">(<a href="#readme-top">başa dön</a>)</p>

## Başlarken

Betiği tarayıcınızda çalıştırmak için aşağıdaki adımları izleyin.

### Gereksinimler

* Tampermonkey gibi bir kullanıcı betiği yöneticisi
  ```
  Chrome, Edge, Firefox, Safari ve diğerleri: https://www.tampermonkey.net/
  ```

### Kurulum

1. Tarayıcınıza [Tampermonkey](https://www.tampermonkey.net/) eklentisini kurun.
2. Tampermonkey içinde yeni bir betik oluşturun.
3. [`betik.js`](betik.js) dosyasının içeriğini kopyalayıp yeni betiğe yapıştırın.
4. Betiği kaydedin ve etkin olduğundan emin olun.

<p align="right">(<a href="#readme-top">başa dön</a>)</p>

## Kullanım

1. [https://www.reddit.com/subreddits/](https://www.reddit.com/subreddits/) adresini (veya `old.reddit.com/subreddits/`) açın.
2. Kontrol panelinin sayfada belirmesini bekleyin.
3. Bir hız ayarı seçin. Büyük abonelik listelerinde "Normal" veya "Yavaş" seçeneği önerilir.
4. İşlemi başlatmak için "BAŞLAT" butonuna tıklayın. Süreci "DURAKLAT" ve "DEVAM ET" ile yönetebilirsiniz.
5. Paneli yerini değiştirmek için başlığından tutup sürükleyin.

<p align="right">(<a href="#readme-top">başa dön</a>)</p>

## Teknik Notlar

Betik, alt dizin sayfasında toplu DOM etkileşimi gerçekleştirir. Büyük listelerde istekleri stabil tutmak için daha yavaş bir hız ayarı kullanın. İşlem tamamlanana kadar sayfayı açık tutun.

<p align="right">(<a href="#readme-top">başa dön</a>)</p>

## Katkıda Bulunma

Katkılarınız memnuniyetle karşılanır. Projeyi daha iyi hale getirecek bir öneriniz varsa depoyu fork edip bir pull request açabilir ya da "enhancement" etiketiyle bir issue oluşturabilirsiniz.

1. Projeyi fork edin
2. Özellik dalınızı oluşturun (`git checkout -b feature/AmazingFeature`)
3. Değişikliklerinizi commit edin (`git commit -m 'Add some AmazingFeature'`)
4. Dalınızı push edin (`git push origin feature/AmazingFeature`)
5. Bir Pull Request açın

<p align="right">(<a href="#readme-top">başa dön</a>)</p>

## İletişim

Ayberk - [@aybrkaknc](https://github.com/aybrkaknc)

Proje Bağlantısı: [https://github.com/aybrkaknc/RedditUnfollowAllScript](https://github.com/aybrkaknc/RedditUnfollowAllScript)

<p align="right">(<a href="#readme-top">başa dön</a>)</p>

## Teşekkürler

* [Best-README-Template](https://github.com/aybrkaknc/Best-README-Template)

<p align="right">(<a href="#readme-top">başa dön</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/aybrkaknc/RedditUnfollowAllScript.svg?style=for-the-badge
[contributors-url]: https://github.com/aybrkaknc/RedditUnfollowAllScript/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/aybrkaknc/RedditUnfollowAllScript.svg?style=for-the-badge
[forks-url]: https://github.com/aybrkaknc/RedditUnfollowAllScript/network/members
[stars-shield]: https://img.shields.io/github/stars/aybrkaknc/RedditUnfollowAllScript.svg?style=for-the-badge
[stars-url]: https://github.com/aybrkaknc/RedditUnfollowAllScript/stargazers
[issues-shield]: https://img.shields.io/github/issues/aybrkaknc/RedditUnfollowAllScript.svg?style=for-the-badge
[issues-url]: https://github.com/aybrkaknc/RedditUnfollowAllScript/issues
[tampermonkey-shield]: https://img.shields.io/badge/userscript-Tampermonkey-00485B?style=for-the-badge
[tampermonkey-url]: https://www.tampermonkey.net/
[JavaScript-shield]: https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black
[JavaScript-url]: https://developer.mozilla.org/en-US/docs/Web/JavaScript
[Tampermonkey-badge]: https://img.shields.io/badge/Tampermonkey-00485B?style=for-the-badge
[Tampermonkey-url]: https://www.tampermonkey.net/
