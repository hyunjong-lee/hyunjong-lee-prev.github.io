---
layout: post
title:  Gaming on AWS Hackathon 참가 후기
date:   2016-09-25 10:53:24
categories: Tech
---

본 포스팅은 [Gaming on AWS 해커톤] 행사 참관 후기 및 구현 내용에 대한 간략한 설명을 담고 있습니다.
![Gaming on AWS Hackerton](/assets/images/aws_hackerthon_2016/gamingonaws__hackathon.png)


작년 지인의 소개로 [Gaming on AWS 해커톤] 행사를 알게 되었는데 올해도 행사가 열린다기에 참가하기로 결정하고 친구들과 의기투합하였습니다.
지난해와 마찬가지로 서버 없는 (Serverless) 구조를 통한 게임 플랫폼 개발을 하는 것이 주제였습니다.

아래 포스팅을 보시면 작년에 진행한 내용을 확인하실 수 있습니다.
[작년 참가후기]({% post_url 2015-09-16-AWS-Lambda-Serverless-Turn-Game %})

제시된 주제는 다음과 같았습니다. 작년과 크게 다르지 않습니다.

  * NoSQL을 EC2에 직접 설치하지 않고 DynamoDB를 이용
  * Back-end API server를 직접 구성하는 대신 API Gateway와 Lambda를 이용
  * S3를 스토리지로 적극 활용
  * Cognito, SNS, Mobile Analytics를 활용


### 게임 선정

대회를 참가하기로 결정한 날, 대회 1주전, 그리고 대회 당일 이렇게 3번 친구들과 오프라인으로 모였는데 <del>단 한번도 빼놓지 않고 공돌이 특유의 개그가 오갑니다</del> 실시간성이 높은 게임을 목표로 이야기를 나누었습니다.
작년 참가시엔 이제 막 람다 서비스가 나온 상태였고 Seoul Region에 서비스가 없는 상태였기 때문에 실시간 대전 게임이 아닌 턴제 게임을 목표로 하였지만 올해는 한번 제대로 미쳐보기로 했습니다.


https://www.assetstore.unity3d.com/kr/#!/content/13866

https://www.youtube.com/watch?v=kX0hnOS1QQQ



### AWS Architecture 구성

2016년 시스템 구성도

![Dodge AWS Architecture](/assets/images/aws_hackerthon_2016/architecture.png)


2015년 시스템 구성도

![Ataxx AWS Architecture](/assets/images/aws_hackerton/architecture.png)



물론 이런 구조는 <del>저같은 초짜는 할 수 없는</del> AWS에 경험많은 친구의 조언을 통해 나왔습니다.


### 대회 당일


![행사장 모습](/assets/images/aws_hackerthon_2016/contest_day_morning.jpg){: .img}




행사 끝나고 단체사진을 찍었는데 작년엔 얼굴이 잘려나와서 올해는 신중히 자리를 정했고 다행이 얼굴이 다 나왔습니다!
![행사 끝나고 찍은 단체사진](/assets/images/aws_hackerthon_2016/pic2.jpg){: .img}

`각 팀의 발표를 들으며 제가 어떤 행사에 왔는지 다시금 깨달았습니다.` 라고 작년에 적어두었는데 올해도 같은 느낌이었습니다.
모든 분들이 게임을 잘 만들어 오셨는데 저희팀은 시스템 구성을 먼저 한 후 게임은 대회장에서 만들었습니다.
미친 기획력을 보여준 친구와 클라 개발이 가능한 친구들이 합류하여 별다른 실수없이 게임이 챡챡 완성되었습니다.

팀웍이 좋았는지 올해도 수상을 하였습니다. 작년과 같이 2등을 하였는데 올해도 2등 상품은 에코입니다.

![2등 상품 amazon echo](/assets/images/aws_hackerthon_2016/echo.jpg){: .img}


왜인진 모르겠는데 자꾸 콩진호라는 단어가 머리속에서 맴돕니다

![자꾸 떠오르는 콩진호](/assets/images/aws_hackerthon_2016/kong.jpg){: .img}


[Gaming on AWS 해커톤]: https://aws.amazon.com/ko/events/gaming-on-aws/seoul-02/hackathon/
[세균전]: https://en.wikipedia.org/wiki/Ataxx