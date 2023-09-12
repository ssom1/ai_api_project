# BARD와 CHATGPT 를 활용한 문서요약 API



## 1. 개요
***
이번 프로젝트에서는 자연어 처리 API를 활용해서 신문 기사 내용을 요약해서 보여주는 서비스를
해보자고 한다. 신문 기사는 우리에게 유용한 정보를 제공하고 있으나, 때에 따라서는 간단하게 핵심만 알기를 원한다. 네이버, 다음, 구글 등 다양한 플랫폼에서는 이미 신문기사 요약 기능을 제공하고 있으나, 이번 프로젝트에서는 어떠한 신문 기사도 요약을 해줄 수 이쓴 서비스를 구현해볼 것이다. 이 서비스의 입력은 신문 기사의 인터넷 주소(url)이고, 출력은 해당 기사의 요약문이 될 것이다.



## 2.활용한 인공지능 API
BARD에서는 문장을 해석하는 API ,CHATGPT에서는 질문분석 API를 사용하였다
*** 
### 2.1 API의 입력과 출력
BARD = ~이 기사문을 요약해줘(기사문은 길어서 생략)
CHAT GPT = 문서 요약 API가 뭔지 설명해줘
### 2.2문서요악 API
chatgpt를 이용한 문서요약 API의 기능과 설명 글 이다.

"문서 요약 API"는 텍스트 기반 문서나 글을 자동으로 요약하는 데 사용되는 응용 프로그램 프로그래밍 인터페이스(API)입니다. 이 API를 통해 개발자는 다음과 같은 주요 작업을 수행할 수 있습니다:

1. **텍스트 요약**: 문서 요약 API를 사용하면 긴 텍스트 문서를 간결하게 요약할 수 있습니다. 이는 정보 과부하를 줄이고 독자 또는 사용자에게 중요한 내용을 제공하는 데 도움이 됩니다.

2. **자동 요약**: API는 인공 지능 기술을 사용하여 문서의 핵심 내용을 식별하고 중요한 문장이나 단어를 추출하여 요약합니다. 이렇게 하면 수작업으로 요약하는 시간과 노력을 절약할 수 있습니다.

3. **다국어 지원**: 일부 문서 요약 API는 다양한 언어를 지원하며, 다국어 텍스트의 요약을 수행할 수 있습니다.

4. **특정 도메인에 대한 요약**: 특정 주제나 도메인에 관련된 문서를 요약하는 데 특화된 API도 있습니다. 예를 들어 의학, 금융, 기술 등의 분야에 특화된 요약 기능을 제공할 수 있습니다.

5. **요약 길이 설정**: API를 사용하는 개발자는 요약 결과의 길이를 조절할 수 있으며, 요약 문장 수나 글자 수를 제한할 수 있습니다.

문서 요약 API는 다양한 응용 분야에서 사용될 수 있습니다. 예를 들어 뉴스 기사, 논문, 블로그 게시물, 리뷰 등의 긴 텍스트를 간단하게 요약하여 독자들에게 정보를 제공하거나, 정보 검색 시스템에서 검색 결과를 개선하고, 정보 추출 및 분석 작업을 자동화하는 데 활용됩니다. 이러한 API는 개발자들이 복잡한 요약 알고리즘을 구현하지 않고도 텍스트 요약을 쉽게 통합할 수 있도록 도와줍니다.
## 3.웹페이지 구축

### 3.1기사 내용 추출하기
대전의 한 초등학교 교사가 숨진 사건과 관련해, 교사를 괴롭힌 것으로 지목된 학부모들의 신상이 SNS에서 폭로됐습니다.

학부모의 이름, 전화번호, 사업장, 가족 사진까지 공개되면서, '정의구현'을 외치는 댓글이 이어졌지만, 2차 피해를 우려하는 목소리도 나오고 있습니다.

한편, 가해자로 지목된 학부모 중 한 명은 자신이 교사를 괴롭힌 적이 없다고 주장하며, 신상 털기와 허위사실 유포를 중단해달라고 호소했습니다.

숨진 교사는 2019년 동급생을 폭행한 학생을 교장실에 보냈다는 이유로 악성 민원에 시달렸고, 2020년에는 아동학대 혐의로 고소까지 당했습니다. 무혐의 처분을 받은 뒤 올해 근무지를 옮겼지만, 최근 발생한 다른 교사 사망 사건 이후 트라우마를 호소하다 지난 5일 자택에서 스스로 목숨을 끊었습니다.

요약하면, 숨진 초등학교 교사가 악성 민원에 시달리다가 극단적 선택을 한 사건과 관련해, 교사를 괴롭힌 것으로 지목된 학부모들의 신상이 SNS에서 폭로됐습니다. 2차 피해를 우려하는 목소리도 나오는 가운데, 가해자로 지목된 학부모 중 한 명은 자신이 교사를 괴롭힌 적이 없다고 주장하고 있습니다.

### 3.2외국어일 경우 한국어로 번역하는 기능추가
XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
### 3.3웹페이지 구성


## 4.실행결과
