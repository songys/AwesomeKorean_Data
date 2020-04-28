# Awesome_Korean_Data
한국어 데이터 세트 링크

팁: ragsgo 전처리 데이터 [:octocat:](https://ratsgo.github.io/embedding/preprocess.html)에서는 한국어 위키피디아를 포함한 전처리 데이터와 위젯을 이용한 데이터 다운로드를 제공하고 있음!


# 한국어 텍스트 데이터       
|번호|데이터 종류| 링크| 비고|
|:---:|:-----------------:|:-----------------:|:-----------------:|
|1.|한국 정치인 뉴스 데이터 세트 |[:octocat:](https://github.com/lovit/politician_news_dataset)|-|
|2.|네이버 뉴스 중 IT/과학 분야에서 50개를 선정해서 요약에 해당하는 문장을 태깅해둔 데이터 세트 |[:octocat:](https://github.com/theeluwin/sci-news-sum-kr-50)|-|
|3.|영화추천시스템을 위한 데이터 세트 |[:octocat:](https://github.com/lovit/kmrd)|-|
|4.|Naver sentiment movie corpus v1.0(네이버 악평과 선평을 구분해 놓은 데이터)| [:octocat:](https://github.com/e9t/nsmc)|-|
|5.|Naver sentiment movie corpus v1.0를 다운 받아서 감성분석 레이블링을 상세화('toxic', 'obscene', 'threat', 'insult', 'identity_hate')한 데이터 |[:octocat:](https://github.com/songys/Toxic_comment_data)|-|
|6.|Paired Question(질문쌍이 같은 질문인지 다른 질문인지 구별하는 데이터)|[:octocat:](https://github.com/songys/Question_pair)|-|
|7.|한국어 개체명 정의 및 표지 표준화 기술보고서와 이를 기반으로 제작된 개체명 형태소 말뭉치|[:octocat:](https://github.com/kmounlp/NER)|-|
|8.|KoreanNERCorpus(개체명 말뭉치) |[:octocat:](https://github.com/machinereading/KoreanNERCorpus)|-|
|9.|한국어 NER 사전 |[:octocat:](https://github.com/songys/entity)|-|
|10.1| 챗봇용 대화 세트 |[:octocat:](https://github.com/songys/Chatbot_data)|-|
|10.2| 챗봇용 대화 세트와 코드| [:octocat:](https://github.com/warnikchow/paraKQC)|10.1과 10.2는 거의 겹치는 질문이 없다고 할 만큼 주제가 다르다. 10.1은 "위로해 줘"와 같이 좀 더 사적 담화의 성격이 강하다면 10.2는 "어떤 메일이 더 유용해?" 와 같이 지식인 QnA에 나올 법한 질문들도 많다.|
|11.|한영/한불 병렬말뭉치(번역용)|[:octocat:](https://github.com/j-min/korean-parallel-corpora)|-|
|12.|[청와대 국민청원](https://www1.president.go.kr/petitions) 사이트의 [만료된 청원](https://www1.president.go.kr/petitions?only=finished) 데이터 모음| [:octocat:](https://github.com/akngs/petitions)|-|
|13.|공공데이터포털 뉴스빅데이터 분석 정보(뉴스데이터베이스 'Kinds' 기반 분석 자료, 기사 메타정보)|https://www.data.go.kr/dataset/15012945/fileData.do |-|



# 회사나 팀에서 구축한 데이터
|번호|데이터 종류| 링크| 비고|
|:---:|:-----------------:|:-----------------:|:-----------------:|
|1.| Kyubyong Park 외(2019), 한국어 Text to Speech 를 위한 데이터 |https://www.kaggle.com/bryanpark/korean-single-speaker-speech-dataset?fbclid=IwAR1WltCqIATEfpPsglqNgQm4zv6-rkmLvf7XMTJwuQ8nlRvaLpukZhtRhvw |-|
|2.| 질의 응답용 데이터 KorQuAD 2.0 질문답변 20,000+ 쌍을 포함하여 총 100,000+ 쌍으로 구성된 한국어 Machine Reading Comprehension 데이터 세트 |[:octocat:](https://korquad.github.io/)|KorQuAD 데이터 세트와 관련된 설명 동영상 -> https://www.youtube.com/watch?v=ntGwv6Ifoe8 |
|3.| 카카오 브레인에서 발표한 RTE (recognizing text entailment) 데이터 세트 |[:octocat:](https://github.com/kakaobrain/KorNLUDatasets) | -|              


# 국가적 규모에서 구축한 데이터
|번호|데이터 종류| 링크| 비고|
|:---:|:-----------------:|:-----------------:|:-----------------:|          
|1.| 우리말샘 : 다양한 어휘와 유의어 정보 등을 얻을 수 있는 대사전 : 로그일 필요, 전체 사전 데이터 다운로드 가능| https://opendict.korean.go.kr/main| 이 사전에 대한 설명 github [:octocat:](https://github.com/songys/Dictionaries)|      
|2.| 전자 사전 : NIA 사전, 묻지도 따지지도 않고 다음 링크에서 엑셀로 다운로드 가능 |https://kbig.kr/portal/kbig/knowledge/files/bigdata_report.page?bltnNo=10000000016451 |-|
|3.| AIHub : 텍스트와 음성 멀티모달까지 가장 광범위한 데이터, 로그인 및 사용 목적과 기간을 명시한 사용 신청서 작성 후 허가 메일이 오면(하루 정도 걸린다) 다운로드 가능 |http://aihub.or.kr/ |-|                
|4.| 국립국어원 언어정보나눔터 : 로그인 후 세종2007 말뭉치나 낭독체 음성 파일 등도 다운로드 가능, 다운 받을 때 간단한 서약에 체크만 하면 되는데 자료의 크기를 작게 나누어 놓아서 여러번 체크해야 한다는 것이 단점 | https://ithub.korean.go.kr/user/total/database/corpusManager.do |-|       







