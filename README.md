# ☕️ STARBUCKS
### 스타벅스 홈페이지를 만든 예제입니다.</br>

🗓️ 작업기간 : 2022. 01. 24 ~ 2022. 01. 30

👨‍💻 투입인원 : 1명 (개인 프로젝트)

🌱 스킬 및 사용 툴

![HTML5](https://camo.githubusercontent.com/6b971142fed08e462a1fab5b35c9e1d84b454bbfed795abf83836d5ef4c4cb17/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f48544d4c352d2532334533344632362e7376673f7374796c653d666c61742d737175617265266c6f676f3d68746d6c35266c6f676f436f6c6f723d7768697465266d61782d77696474683d31303025)
![CSSS](https://camo.githubusercontent.com/852a0305ff0c2a6b5d10932eef2cfbfb59be3e99ce69002473077b5045344e89/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f435353332d2532333135373242362e7376673f7374796c653d666c61742d737175617265266c6f676f3d63737333266c6f676f436f6c6f723d7768697465)
![javascript](https://camo.githubusercontent.com/9ee5409ea3b88163eeaa617ba53eff2c7610c55618c99dd4bd00bec40e6aee48/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4a6176615363726970742d2532333332333333302e7376673f7374796c653d666c61742d737175617265266c6f676f3d6a617661736372697074266c6f676f436f6c6f723d253233463744463145)
![Netlify](https://camo.githubusercontent.com/4eb846bfdaaa72e0bc1dc3e29898a9b5db55cf1fee11700600333cf29012d15d/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4e65746c6966792d2532333030303030302e7376673f7374796c653d666c61742d737175617265266c6f676f3d6e65746c696679266c6f676f436f6c6f723d23303043374237)
![Git](https://camo.githubusercontent.com/b38b8897560b3731eafccf44bf41f9450b71ec972a7759e0d104402403b51b13/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4769742d2532334630353033332e7376673f7374796c653d666c61742d737175617265266c6f676f3d676974266c6f676f436f6c6f723d7768697465)

[스타벅스 메인 웹 페이지로 이동](https://practical-allen-a945c9.netlify.app/ "스타벅스 메인 웹 페이지로 이동")

[스타벅스 로그인 웹 페이지로 이동](https://practical-allen-a945c9.netlify.app/signin/ 
"스타벅스 로그인 웹 페이지로 이동")

[![스타벅스 메인 웹 페이지](https://raw.githubusercontent.com/ParkYoungWoong/starbucks-vanilla-app/master/_assets/main_screenshot.jpg)](https://practical-allen-a945c9.netlify.app/)

# 문자 인코딩(Character Encoding) 설정
문자가 인코딩되는 방식을 설정합니다.

```html
<meta charset="UTF-8"/>
```
- text - UTF-8: 초성,중성,종성으로 구분하여 문자를 작성(권장)
- EUC-KR: 하나의 완성된 글자를 인식

# 뷰포트(Viewport) 렌더링 방식 설정
웹페이지가 화면(Viewport)에 표현돠는 방식을 설정합니다.
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```
- `width=device-width`: 화면의 가로 너비를 각 디바이스(Device)의 가로 너비와 동일하게 적용
- `initial-scale=1.0`:  화면의 초기 화면 배율(확대 정도)을 설정
- `user-scalable=no`: 사용자가 디바이스 화면을 확대(yes)/축소(no)할 수 있는지 설정
- `maximum-scale=1`: 사용자가 화면을 확대할 수 있는 최댓값
- `minimum-scale=1`: 사용자가 화면을 축소할 수 있는 최솟값

# 오픈 그래프(The Open Graph protocol)
웹페이지가 소셜 미디어(facebook)으로 공유될 때 우선적으로 활용되는 정보를 지정합니다.

Slack - 

![스터벅스](https://raw.githubusercontent.com/ParkYoungWoong/starbucks-vanilla-app/master/_assets/slack_message_og_example.jpg)

KaKaoTalk - 

![카카오톡](https://raw.githubusercontent.com/ParkYoungWoong/starbucks-vanilla-app/master/_assets/kakao_og_example.jpg)

[더 많은 오픈 그래프 속성 보기](https://ogp.me/)
```html
<meta property="og:type" content="website" />
<meta property="og:site_name" content="Starbucks" />
<meta property="og:title" content="Starbucks Coffee Korea" />
<meta property="og:description" content="스타벅스는 세계에서 가장 큰 다국적 커피 전문점으로, 64개국에서 총 23,187개의 매점을 운영하고 있습니다." />
<meta property="og:image" content="./images/starbucks_seo.jpg" />
<meta property="og:url" content="https://starbucks.co.kr" />
```
- `og:type`: 페이지의 유형(E.g, website, video.movie)
- `og:site_name`: 속한 사이트의 이름
- `og:title`: 페이지의 이름(제목)
- `og:description`: 페이지의 간단한 설명
- `og:image`: 페이지의 대표 이미지 주소(URL)
- `og:url`: 페이지 주소(URL)

# 트위터 카드(Twitter Cards)
웹페이지가 소셜 미디어(트위터)로 공유될 때 우선적으로 활용되는 정보를 지정합니다.

[더 많은 트위터 카드 보기](https://developer.twitter.com/en/docs/twitter-for-websites/cards/guides/getting-started)

```html
<meta property="twitter:card" content="summary" />
<meta property="twitter:site" content="Starbucks" />
<meta property="twitter:title" content="Starbucks Coffee Korea" />
<meta property="twitter:description" content="스타벅스는 세계에서 가장 큰 다국적 커피 전문점으로, 64개국에서 총 23,187개의 매점을 운영하고 있습니다." />
<meta property="twitter:image" content="./images/starbucks_seo.jpg" />
<meta property="twitter:url" content="https://starbucks.co.kr" />
```
- `witter:card`: 페이지(카드)의 유형(E.g. summary, player)
- `twitter:site`: 속한 사이트의 이름
- `twitter:title`: 페이지의 이름(제목)
- `twitter:description`: 페이지의 간단한 설명
- `twitter:image`: 페이지의 대표 이미지 주소(URL)
- `twitter:url`: 페이지 주소(URL)

# Favicon(파비콘, favorites icon)
웹페이지를 나타내는 아이콘, 웹페이지의 로고를 설정합니다.
대부분의 경우 루트 경로에 favicon.ico 파일을 위치하면 자동으로 로딩하기 때문에 <link /> 를 작성할 필요가 없습니다. favicon.png 파일을 사용하려면 다음과 같이 <link />를 작성하세요.

> 파비콘 이미지는 루트 경로에 있어야 합니다!
```html
<!--<link rel="shortcut icon" href="favicon.ico" />-->
<link rel="icon" href="./favicon.png" />
```
- favicon.ico 64 x 64 (px) 또는 32 x 32 또는 16 x 16
- favicon.png 500 x 500 (px)

<img src="https://raw.githubusercontent.com/ParkYoungWoong/starbucks-vanilla-app/master/favicon.png" alt="Favicon" width="30%" height="30%">


## .ico 파일 제작
이미지를 업로드하면 손쉽게 .ico 파일을 제작할 수 있습니다.

# Reset.css
각 브라우저의 기본 스타일을 초기화합니다.
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/reset-css@5.0.1/reset.min.css" />
```
# Google Fonts
페이지에서 사용할 '나눔고딕' 폰트를 지정합니다.
> 폰트 라이선스를 꼭 확인해야 합니다!

[Google Fonts](https://fonts.google.com/)
에서 고른 폰트 파일을 가져옵니다.
```html
<link rel="preconnect" href="https://fonts.gstatic.com" />
<link href="https://fonts.googleapis.com/css2?family=Nanum+Gothic:wght@400;700&display=swap" rel="stylesheet" />
```
페이지에 폰트를 적용(CSS 상속)합니다.
```html
body {
    font-family: 'Nanum Gothic', sans-serif;
}
```

# Google Material Icons
[구글에서 제공하는 머터리얼 아이콘](https://fonts.google.com/icons?selected=Material+Icons)을 무료로 사용할 수 있습니다.

다음과 같이 사용할 수 있습니다.
```html
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons" />
```
```html
<div class="material-icons">upload</div>
```
# GSAP & ScrollToPlugin (순차적 에니메이션)
[GSAP(The GreenSock Animation Platform)](https://greensock.com/gsap/)
은 자바스크립트로 제어하는 타임라인 기반의 애니메이션 라이브러리입니다.
[ScrollToPlugin](https://greensock.com/scrolltoplugin/)은 스크롤 애니메이션을 지원하는 GSAP 플러그인입니다.

```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.5.1/gsap.min.js" integrity="sha512-IQLehpLoVS4fNzl7IfH8Iowfm5+RiMGtHykgZJl9AWMgqx0AmJ6cRWcB+GaGVtIsnC4voMfm8f2vwtY+6oPjpQ==" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.5.1/ScrollToPlugin.min.js" integrity="sha512-nTHzMQK7lwWt8nL4KF6DhwLHluv6dVq/hNnj2PBN0xMl2KaMm1PM02csx57mmToPAodHmPsipoERRNn4pG7f+Q==" crossorigin="anonymous"></script>
```
[.to() 사용법](https://greensock.com/docs/v3/GSAP/gsap.to()) [GSAP Easing](https://greensock.com/docs/v2/Easing)

```javascript
gsap.to(요소, 시간, 옵션)
// 또는
TweenMax.to(요소, 시간, 옵션)
```
```javascript
gsap.to(window, .7, {
  scrollTo: 0
});
```
```javascript
// 화면 스크롤 이벤트 발생시 배지 및 버튼 숨기기

const badgeEl = document.querySelector('header .badges')

const toTopEl = document.querySelector('#to-top');

// _.throttle(함수, 시간);

window.addEventListener("scroll", _.throttle(function () {

if(window.scrollY > 500) { // 배지 숨기기

// gsap.to(요소, 지속시간, 옵션);

gsap.to(badgeEl, 0.6, {

opacity: 0, // 투명도

display: 'none'

});

// 버튼 보이기

gsap.to(toTopEl, 0.2, {

x: 0

});

} else { // 배지 보이기

gsap.to(badgeEl, 0.6, {

opacity: 1,

display: 'block'

});

// 버튼 숨기기

gsap.to(toTopEl, 0.2, {

x: 100

});

}

}, 300));

toTopEl.addEventListener('click', function() {

gsap.to(window, 0.7, {

scrollTo: 0 // 스크롤을 0px 위치로 옮김

});

})

// 순차적으로 요소 보이기

const fadeEls = document.querySelectorAll('.visual .fade-in');

fadeEls.forEach(function (fadeEl, index) {

// gsap.to(요소, 지속시간, 옵션);

gsap.to(fadeEl, 1, {

delay: (index + 1) * 0.7, // 0.7, 1.4, 2,.1, 2.7

opacity: 1

});

});
```
# Swiper (화면 전환)
[Swiper](https://swiperjs.com/)는 하드웨어 가속 전환과 여러 기본 동작을 갖춘 현대적인 슬라이드 라이브러리입니다.</br>

[Getting Started With Swiper](https://swiperjs.com/get-started)

```html
<!-- in HEAD -->
<link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css" />
<script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>

<!-- in BODY -->
<div class="swiper-container">
  <div class="swiper-wrapper">
    <div class="swiper-slide">1</div>
    <div class="swiper-slide">2</div>
    <div class="swiper-slide">3</div>
  </div>
</div>
```
[Swiper API](https://swiperjs.com/swiper-api)(옵션)을 확인하세요!

```javascript
new Swiper(선택자, 옵션);
```
```javascript
new Swiper('.swiper-container', {
  direction: 'vertical', // 수직 슬라이드
  autoplay: true, // 자동 재생 여부
  loop: true // 반복 재생 여부
});

// 요소 수평 슬라이드 만들기 (NOTICE)
new Swiper('.promotion .swiper-container', {
slidesPerView: 3, // 한번에 보여줄 슬라이드 개수
spaceBetween: 10, // 슬라이드 사이 여백
centeredSlides: true, // 1번 슬라이드가 가운데 보이기
loop: true,
autoplay: { delay: 5000 },
pagination: {
el: '.promotion .swiper-pagination', // 페이지 번호 요소 선택자
clickable: true // 사용자의 페이지 번호 요소 제어 가능 여부
},
navigation: {
prevEl: '.promotion .swiper-prev', // 이전 요소
nextEl: '.promotion .swiper-next' // 다음 요소
}
});
```
# Youtube API
[IFrame Player API](https://developers.google.com/youtube/iframe_api_reference?hl=ko)를 통해 YouTube 동영상을 제어할 수 있습니다.

유튜브 영상이 출력될 위치에 요소를 지정(생성)합니다.
```html
<!-- in HEAD -->
<script defer src="./js/youtube.js"></script>

<!-- in BODY -->
<!-- YOUTUBE VIDEO -->
<section class="youtube">
<div class="youtube__area">
<div id="player"></div>
</div>
<div class="youtube__cover"></div>
<div class="inner">
<img src="./images/floating1.png" alt="Icon" class="floating floating1">
<img src="./images/floating2.png" alt="Icon" class="floating floating2">
</div>
</section>
```
`onYouTubePlayerAPIReady` 함수 이름은 Youtube IFrame Player API에서 사용하는 이름이기 때문에 다르게 지정하면 동작하지 않습니다!
그리고 함수는 전역(Global) 등록해야 합니다!

[플레이어 매개변수(playerVars)](https://developers.google.com/youtube/player_parameters.html?playerVersion=HTML5&hl=ko#Parameters)에서 더 많은 옵션을 확인할 수 있습니다.
```javascript
// Youtube IFrame API를 비동기로 로드합니다.
var tag = document.createElement('script');
tag.src = "https://www.youtube.com/iframe_api";
var firstScriptTag = document.getElementsByTagName('script')[0];
firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);

function onYouTubePlayerAPIReady() {
  // <div id="player"></div>
  new YT.Player('player', {
    videoId: 'An6LvWQuj_8', // 재생할 유튜브 영상 ID
    playerVars: {
      autoplay: true, // 자동 재생 유무
      loop: true, // 반복 재생 유무
      playlist: 'An6LvWQuj_8' // 반복 재생할 유튜브 영상 ID 목록
    },
    events: {
      // 영상이 준비되었을 때,
      onReady: function (event) {
        event.target.mute(); // 음소거!
      }
    }
  });
}
```

# ScrollMagic (스크롤 이동)
`ScrollMagic`은 스크롤과 요소의 상호 작용을 위한 자바스크립트 라이브러리입니다.
대표적으로 어떤 요소가 현재 화면에 보이는 상태인지를 확인할 때 사용합니다.

[ScrollMagic API](http://scrollmagic.io/docs/)

```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/ScrollMagic/2.0.8/ScrollMagic.min.js"></script>
```
```javascript
new ScrollMagic
  .Scene({ // 감시할 장면(Scene)을 추가
    triggerElement: spyEl, // 보여짐 여부를 감시할 요소를 지정
    triggerHook: .8 // 화면의 80% 지점에서 보여짐 여부 감시
  })
  .setClassToggle(spyEl, 'show') // 요소가 화면에 보이면 show 클래스 추가
  .addTo(new ScrollMagic.Controller()) // 컨트롤러에 장면을 할당(필수!)
```

# Lodash
[Lodash](https://lodash.com/)는 다양한 유틸리티 기능을 제공하는 자바스크립트 라이브러리입니다.</br>

[Lodash API](https://lodash.com/docs/4.17.15)</br>
[Lodash throttle](https://lodash.com/docs/4.17.15#throttle)
```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/lodash.js/4.17.20/lodash.min.js" integrity="sha512-90vH1Z83AJY9DmlWa8WkjkV79yfS2n2Oxhsi2dZbIv0nC4E6m5AbH8Nh156kkM7JePmqD6tcZsfad1ueoaovww==" crossorigin="anonymous"></script>
```

# 랜덤한 숫자를 생성하는 함수
```javascript
// 범위 랜덤 함수(소수점 2자리까지)
function random(min, max) {
  // `.toFixed()`를 통해 반환된 문자 데이터를,
  // `parseFloat()`을 통해 소수점을 가지는 숫자 데이터로 변환
  return parseFloat((Math.random() * (max - min) + min).toFixed(2))
}
```
# 현재 날짜를 계산하는 함수
```html
<!-- in BODY -->
<p class="copyright">
©<span class="this-year"></span> Starbucks Coffee Company. All Rights Reserved.
</p>
```
```javascript
const thisYear = document.querySelector('.this-year');
thisYear.textContent = new Date().getFullYear(); // 현재 년도의 숫자 데이터 반환(2022)
```
