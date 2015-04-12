# TachyFont 웹폰트 적용 안내
###

## 이 프로젝트는 [TachyFont](https://github.com/googlei18n/TachyFont)를 기반으로 하고 있습니다.

구동 방식 설명
========

기존의 nfont, typeeninge 등의 서브셋용 문자셋 전송 후 매번 서브셋화된 웹폰트 파일을 받는 것이 아니라. 원 저자의 표현을 빌리자면 'Incremental Fonts'입니다. 즉, IndexedDB에 저장되어 있지 않지만 필요한 문자를 그때그때 요청해서 그 글리프 데이터만 누적시켜 폰트 파일과 IndexedDB를 갱신하는 형태입니다.

서버 상태 안내
========

서버는 현재 염가 서버라 언제나 동작한다는 업타임 보장이 없으나 최선을 다해 유지하겠습니다. 이 점은 너그러운 양해를 부탁드립니다. 또한 원 프로젝트 자체가 현재(2015-03-18 기준) 알파버전입니다. 예상치 못한 일이 늘 발생할 수 있으니 이점 유념해주세요 ㅋㅋ

브라우저 지원 안내
===============

관련 상세 사항은 [TachyFont - Browser Support](https://github.com/googlei18n/TachyFont#browser-support)를 참조하시면 되겠습니다. 일반적으로 IndexedDB를 완전히 지원하는 브라우저면 이용이 가능하십니다.

활용법
====================

함께 업로드된 example.html, tachyfont.min.js 파일을 확인해보시면 주석을 함께 달아두었으니 직관적으로 이해 가능하시리라 봅니다.

[예시파일](https://cdn.rawgit.com/c8seki/webfont-tachyfont/e0024c2127135944f0b95bf4fc167ec52a46898a/example.html)을 볼 수 있도록 열어뒀습니다. 확인해보세요!

현재 예제서버는 OpenShift 무료 플랫폼에 업로드 되어 있습니다. 이 서버는 유휴시간이 길 경우 자동으로 꺼지는 기능을 가지고 있습니다. 오랜시간 예제가 로딩이 되지 않는 경우 http://font.cf에 들어가셔서 서버를 깨워주셔야 합니다. ㅋㅋ

폰트 추가 요청
====================

현재 지원되는 폰트는 Fonts 폴더에 들어가시면 안내되어 있습니다.

추가하고 싶으신 폰트셋이 있으시면 본 Github Issues에 문의 바랍니다. 라이센스 확인후 가능한 폰트셋이면 서브셋용 파일로 변환하여 탑재 후 결과를 안내해 드리겠습니다. (당분간은 한글 서체만 가능)

구걸
====================

서버 굴리는데도 비용이 들어갑니다. 운영 겸 확장할 비용을 지원해주시면 감사천만하겠습니다. (물론 안주셔도 똥속도로는 계속 굴러갑니다.) ㅋㅋ

[기부하시려면 여기로 ㄱㄱㄱ](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=4W3BC7TM9HEGG&lc=KR&item_name=Webfont%20Server%20with%20TachyFont&item_number=TACHY1503&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHosted)
