---
layout: post
title:  서평 [C#과 데이터베이스로 누구나 쉽게 주식 자동매매 시스템 만들기]
date:   2017-04-06 01:42:10
categories: Review
---

본 포스팅은 [C#과 데이터베이스로 누구나 쉽게 주식 자동매매 시스템 만들기] 도서에 대한 후기를 담고 있습니다.
자세한 사항은 한빛미디어 홈페이지에서 확인하실 수 있습니다.


### 주식

대학 다닐때 펀드에 가입을 하고 원금을 손실할까 조마조마했던 때가 있습니다.
지금 생각하면 정말 적은 돈이지만 그땐 2주 정도의 학식을 먹을 수 있는 큰돈이었습니다.
<del>(그나마 그 돈도 두달만에 인출해서 밥사먹었다는)</del>

![펀드](/assets/images/trading_system_csharp/fund.jpg){: .img}

- TODO: 펀드와 주식의 연결고리 잘 설명하기

취업한 후엔 카드님과 은행님께서 제 통장을 매달 깨끗이 지워주셨는데요, 최근들어!!! 30대 중반이 되니까!!! 한달에 10만원쯤 여유가 생겼습니다?
이 돈 그냥 넣어두자니 아깝고 해서 주식을 해볼까해서 주변 사람에게 물어보니 PER, ROE, 양봉차트, 물타기 등 모르는 용어 천지였습니다. @_@
<del>데이터쟁이인</del> 저의 관점에선 믿기 어려운 설명들도 있었는데요, 이걸 이해해서 실제로 테스트 해보고 싶은 욕망이 끓어올랐습니다.

그래서 무작정 [머신러닝을 이용한 알고리즘 트레이딩 시스템 개발] 이라는 책을 사버렸습니다!
책을 사고 따라하려는데 실제 매매 시스템을 구축하려보니 증권사에서 제공하는 API의 명세가 너무 많고 용어도 다양해서 이걸 다 볼 엄두가 나지 않았습니다.
공부를 꽤 해야지만 완성할 수 있을 것 같아 지레겁을 먹고 시작하지 못하였는데 페이스북에 [C#과 데이터베이스로 누구나 쉽게 주식 자동매매 시스템 만들기] 라는 책이 출간되었음을 알려주더군요.
인생 뭐 있습니까? 하고 싶은게 있고 재료도 있다면 그냥 하면 되는거죠!


### C#과 데이터베이스로 누구나 쉽게 주식 자동매매 시스템 만들기

![C#과 데이터베이스로 누구나 쉽게 주식 자동매매 시스템 만들기](/assets/images/trading_system_csharp/cover.jpg){: .img}

이 책에서 기대한 내용은 다음과 같았습니다.

- API연동을 어떻게 해야하는지
- 주의해야 할것이 무엇인지
- 복잡한 용어없이 실제로 돌아가는 시스템을 구축할 수 있는지

이 책을 한줄로 요약하자면 위 3가지 질문에 대해 아주 잘 답변을 해준 책이라고 할 수 있습니다.

- TODO: 책 구성과 내용 설명
- TODO: 리뷰어의 주관적인 평가
- TODO: 책의 장점 단점 및 판단의 기준
- TODO: 적절한 짤방을 찾아 집어넣기


~~~ git
commit 4685e4c39eb51ac2e8fe77cc2195cb3ef93819f4
Author: - <-@-.com>
Date:   Tue Mar 28 00:52:47 2017 +0900

    display account info in UI & assertion check for number of accounts and account list data

commit 7a6e1c385dc25ec874e0f992a3e308651e3724cc
Author: - <-@-.com>
Date:   Wed Mar 22 00:44:39 2017 +0900

    implemented login & logout

commit a67eadfa4559077cc93b45d43534182582e7ef00
Author: - <-@-.com>
Date:   Tue Mar 21 23:27:15 2017 +0900

    implemented Logger & remove NLog package

commit 34d8009a248eb8ca108e61bbbbe7e252da823566
Author: - <-@-.com>
Date:   Tue Mar 21 11:06:25 2017 +0900

    UI relocation & log package appended (NLog)

commit 68d7e69064c458adb128dd22c2a20a7ca4f34df0
Author: - <-@-.com>
Date:   Tue Mar 21 08:36:47 2017 +0900

    Initial UI configuration & program icon resources

commit f9811738289ff4f5e8e4d648979e5a43fed72d83
Author: - <-@-.com>
Date:   Tue Mar 21 07:42:39 2017 +0900

    add COM object to using Trading System API

commit 03857cba824744d9dc145232fd87861299d3d869
Author: - <-@-.com>
Date:   Tue Mar 21 07:39:18 2017 +0900

    initial database tables on MySQL

commit b95695669d5576eb607998f377b548617ed99bf2
Author: - <-@-.com>
Date:   Tue Mar 21 07:36:48 2017 +0900

    create admin project & gitignore for VisualStudio
~~~

위는 실제로 local git을 구축한 후 커밋한 로그인데 아침에 시간날 때, 퇴근하고 틈날 때, 혹은 휴가쓰고 놀다가 생각날 때 책을 보며 짬짬이 구현하고 있습니다.
현재 책에서 설명한 내용의 70%쯤 구현된 상태인데 책에서 설명한 대로 시스템을 구축했으면 구현이 끝났을 것 같습니다.

C#의 경우 초보자를 위해서 설명해 두신 내용이 나쁘지 않지만 Oracle의 경우는 MySQL로 설명했으면 어땠을까 하는 아쉬움이 살짝 남습니다.
아래는 제가 개인적으로 느낀 아쉬운 부분인데 이런 부분이 결코 책의 핵심을 훼손하고 있진 않습니다.

- C#
  - C#으로 밥먹고 살던때가 있던지라 책의 로직을 C# 언어 특징을 고려하여 보기좋게(?) 고치고 있습니다.
  - 예를 들면 Extension 메소드 사용, DateTime을 string으로 변환하지 않고 바로 비교
- 데이터베이스
  - 오라클 기준으로 설명하고 있는데 개인용 컴에 깔기엔 상당히 무거운 녀석이라 MySQL을 기반으로 작업을 진행했습니다.
  - 불필요한 필드 정리와 네이밍을 제가 원하는 스타일로 통일했습니다.
  - 책에서는 SQL쿼리를 string 조합으로 사용했는데요 저는 [linq2db]라는 걸 활용해서 ORM 비스무리하게 사용할 수 있도록 변경했습니다.

![더 이상의 자세한 설명은 생략한다](/assets/images/meme/no_any_more_explanation.jpg){: .img}


### 마무리

좋은 책을 읽으면 항상 열정이 불타오르게 되는 것 같습니다.
주식 자동매매 시스템 구축에 있어 제가 가렵던 부분을 긁어준 책이라 재밌게 읽으며 금방 따라할 수 있었습니다.

TODO: 마무리 작성 및 재밌게 잘하기


[C#과 데이터베이스로 누구나 쉽게 주식 자동매매 시스템 만들기]: http://www.hanbit.co.kr/store/books/look.php?p_code=E1054933296
[머신러닝을 이용한 알고리즘 트레이딩 시스템 개발]: http://www.hanbit.co.kr/store/books/look.php?p_code=E2817314825
[linq2db]: https://github.com/linq2db/linq2db