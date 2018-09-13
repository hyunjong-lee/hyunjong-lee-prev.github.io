---
layout: post
title:  삼성 AI 포럼 - 2일차 리뷰
date:   2018-09-13 17:03:28
categories: Review
---


## 주제: Living and Flourishing with Social Robots (Keynote 1)

### 발표자: Cynthia Breazeal | MIT Media Lab
- 관련 영상: https://youtu.be/U1G08KygPVc

#### Relational AI 라는 개념을 소개
- 수학의 Relation이 연관 검색어로 뜨는데 그것과는 다름
- 사람과의 관계를 형성하기 위한 AI 를 말함
- 실제 Product가 있음: https://www.jibo.com/
 
#### 로봇을 잘 만들기 위해 필요한 것
- 사람이 가진 감정과 행동을 이해해야 하며 왜 그러했는지 문맥까지 이해해야 함
- 사람과 AI 간의 UX를 디자인해야 함 (AI 기술 뿐 아니라 사람과의 접점도 중요)
- AI 와 ML 의 혁신


#### 아래 슬라이드가 발표의 핵심을 담고 있음

- ![Relational AI](/assets/images/samsung_ai_forum/relational_ai.jpg)


## 주제: The Computer and the Brain: a Contemporary Perspective (Keynote 2)

### 발표자: Sebastian Seung | Samsung Research & Princeton University
- 관련 영상: https://www.ted.com/talks/sebastian_seung/transcript?language=en

#### 뇌를 nm 단위로 촬영해서 렌더링하고 어떻게 동작하는지 밝히기 위한 연구 과제 공유
- https://www.iarpa.gov/index.php/research-programs/neuroscience-programs-at-iarpa

#### 모세혈관, 미토콘드리아 및 실제 뉴런의 모양을 보여주며 강연 시작
- ![Real Neuron](/assets/images/samsung_ai_forum/neuron.jpg)
- 1px이 nm 단위임을 알려주며 강렬하게 시작
- 분홍색 모양은 하나의 뉴런을 visualize 한 결과

#### 뉴런을 모니터링하며 얻은 교훈을 실제 수식으로 적용
- ![Neuron to Equation](/assets/images/samsung_ai_forum/neuron_equation.jpg)
- 실제 뉴런에서 신호가 너무 강하면 완화하고 너무 약하면 좀 더 강하게 함을 발견하고 이를 수식으로 풀어봄
- 관련자료: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4206525/


## 주제: The Missing Representation in Neural Language Models (Language & Inference 1)

### 발표자: Yejin Choi | University of Washington

- 관련 영상: https://www.microsoft.com/en-us/research/video/nw-nlp-2018-ben-taskar-invited-talk-learning-reasoning-world-using-language/

#### 아마존에서 2017년에 진행한 Alexa 대회에서 우승
- https://www.washington.edu/news/2017/11/28/uw-students-win-amazons-inaugural-alexa-prize-for-most-engaging-and-conversant-socialbot/

#### 기존 모델 (Language Model) 은 사용자와 대화하는데 있어 문제가 있음
- 번역의 경우 상호 연관성을 mapping하는 문제이기에 기존 모델로 잘 풀수 있음
- 상황에 적절한 답변을 하는 경우 대화의 문맥 및 개념 (Common Sense) 등 World에 대한 이해가 필요
  - https://arxiv.org/abs/1612.03969
  - https://arxiv.org/abs/1805.06939
  - http://aclweb.org/anthology/P18-1213

#### L2W (Language 2 Write) 모델을 설명해주며 기존 방식의 생성모델 (LSTM, GRU) 의 결과물과 비교하며 기존보다 좋은 결과가 나옴을 보임
- 특히 사용자 평가에서는 2배이상 좋은 점수를 얻고 있음
- ![Language to Write, L2W](/assets/images/samsung_ai_forum/l2w.jpg)

#### 각종 결과물에 대한 github repo
- https://github.com/uwnlp