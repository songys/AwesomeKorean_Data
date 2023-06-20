
# AwesomeKorean_Data

- 2020년까지 많은 데이터가 구축되었다. 그 중에서 비교적 대부분의 사람들이 접근할 수 있는 오픈 데이터를 정리하였다. 구할 수 있는 모든 데이터를 쏟아 부어서 end to end로 모델을 만들어 보겠다는 포부를 가진 분들의 진입을 쉽게하기 위한 목적이고, 정교한 데이터 구축을 위해서는 이후에 어떠한 데이터가 필요한지를 살펴보기 위한 과정이다.            

- 12월 15일 첫번째 버전을 만들었고 이후 박조은님의 코멘트 그리고 2020년 8월 21일 @warnikchow님의 다양한 기여와 의견을 반영하여 수정하였고 2020년 10월 18일 [메인 레포](https://github.com/ko-nlp/Open-korean-corpora)를 이동하였다. 메일 레포에서는 영어 버전을, 이 곳에는 한국어로 데이터 링크와 약간의 설명을 추가하여 두 가지 버전으로 운영 중이다.   


- Natural language processing의 각 분야에 대한 자료 정리는 다음 링크를 참고     [Awesome-Korean-NLP](https://github.com/datanada/Awesome-Korean-NLP)   


- 다양한 전처리 및 다운로더를 포함한 데이터 링크는 다음을 참조 [https://ratsgo.github.io/embedding/preprocess.html](https://ratsgo.github.io/embedding/preprocess.html)      

- 코퍼스 패키지에 많은 관심이 필요합니다! 웹에 공개되어 있는 한국어 텍스트 데이터들을 손쉽게 로딩하고, 이를 이용하여 모델링한 후 evaluation 까지 편하게 수행하는 / 즉 한국어 텍스트 데이터를 위한 huggingface.nlp 작업 중인 페이지는 다음을 참조, [ko-nlp](https://github.com/ko-nlp/Korpora)
                                    
# Open Datasets
![network](./network.jpg)

- Commercially available(com), academic use only(Academia), unknown(unk)
- Redistribution is possible with or without modification, if neither, or unknown (rd, rd/mod-x, no, unk)  
- Internationally available publication(inter) 


|No.|Dataset|Typical Usage|Provider|Docu.|License|Redist|mod-x|Volume|Goal|Lang.|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
KLUE|Benchmark studies|Industry|int'l|all|rd|0|DP - 15K (s), DST - 10K (d), MRC - 29K (p), NER - 31K (s), NLI - 30K (p), RE - 48K (s), STS - 13K (p), TC - 64K (s)  
KoBEST|Benchmark studies|Industry|int'l|all|rd|0|BoolQ - 6K (p), COPA - 5K (s), KB-WiC - 6K (s), KB-HellaSwag - 3K (p & s), SentiNeg - 4K (s)
KAIST Morpho-Syntactically Annotated Corpus|Morphological analysis|Academia|paper|academic|no|0|70M (w)
OpenKorPOS|Morphological analysis|Academia|int'l|all|rd|0|55M(w)
KAIST Korean Tree-Tagging Corpus|Tree parsing|Academia|int'l|academic|no|0|30K (s)
UD Korean KAIST|Dependency parsing|Academia|int'l|academic|no|1|27K (s)
PKT-UD|Dependency parsing|Academia|int'l|academic|no|0|5K (s)
KMOU NER|NER|Academia|paper|academic|rd|0|24K (s)
AIR x NAVER NER|NER|Competition|docu|academic|no|0|90K (s)
AIR x NAVER SRL|SRL|Competition|docu|academic|no|0|35K (s)
KoNEC & KoNNEC|NER|Academia|docu|academic|no|0|26K(s)
Question Pair|Paraphrase detection|Academia|docu|all|rd|0|10K (p)
KorNLI|NLI|Industry|int'l|all|rd|0|1,000K (p)
KorSTS|STS|Industry|int'l|all|rd|0|8,500K (p)
ParaKQC|Paraphrase detection|Academia|int'l|all|rd|0|540K (p)
StyleKQC|Paraphrase detection|Academia|int'l|all|rd|0|30K(s)
Korean Smile Style Dataset|Paraphrase detection|Industry|docu|academic|rd|0|2,5K(d)
NSMC|Sentiment analysis|Academia|docu|all|rd|0|150K / 50K (s)
Kocasm|Sentiment analysis|Academia|docu|all|rd|0|9K (s)
BEEP!|Hate speech detection|Academia|int'l|all|rd|0|8K / 0.5K / 1K (s)
APEACH|Hate speech detection|Academia|int'l|all|rd|0|4K
Unsmile|Hate speech detection|Industry|docu|academic|rd|0|19K
HateScore|Hate speech detection|Academia|int'l|academic|rd|1|35K
KOLD|Hate speech detection|Academia|int'l|all|rd|0|40K
DKTC|Hate speech detection|Industry|docu|academic|rd|0|1.5K
K-MHaS|Hate speech detection|Academia|int'l|all|rd|0|109K
3i4K|Speech act classification|Academia|int'l|all|rd|0|55K / 6K (s)
KorQuAD 1.0|QA|Industry|int'l|all|rd|1|60K / 5K / 4K (p)
KorQuAD 2.0|QA|Industry|paper|all|rd|1|80K / 10K / 10K (p)
HuLiC|Dialog|Industry|docu|academic|rd|0|115K
OPELA|Dialog|Industry|int'l|academic|rd|0|560K (d)
Sci-news-sum-kr|Summarization|Academia|docu|academic|rd|0|50K (p)
sae4K|Summarization|Academia|int'l|all|rd|0|50K (p)
Korean Parallel Corpora|MT|Academia|int'l|all|rd|1|100K (p)
KAIST Translation Evaluation Set|MT|Academia|docu|academic|no|0|3K (p)
KAIST Chinese-Korean Multilingual Corpus|MT|Academia|docu|academic|no|0|60K (p)
Transliteration Dataset|Transliteration|Academia|docu|all|rd|0|35K (p)
KAIST Transliteration Evaluation Set|Transliteration|Academia|docu|academic|no|0|7K (p)
SIGMORPHON G2P|G2P conversion|Competition|int'l|all|rd|0|3.6K/ 0.45K / 0.45K (p)
PAWS-X|Paraphrase detection|Industry|int'l|all|rd|0|5K / 2K / 2K (p)
TyDi-QA|QA|Industry|int'l|all|rd|0|11K / 1,7K / 1,7K(p)
XPersona|Dialog|Academia|int'l|all|rd|0|0.3K(d) / 4.7K (s)
CareCall|Dialog|Industry|int'l|academic|rd|0|10K
MultiCoNER|NER|Competition|int'l|all|rd|0|178K / 2.6K (s)
Multilingual Tweet Intimacy Analysis|Sentiment analysis|Competition|int'l|unk|unk|0|2K(instances)
IWSLT 2023|MT|Competition|int'l|all|rd|0|3K (p)
KSS|ASR|Academia|docu|academic|rd|0|12+ (h) / 13K (u) / 1 speaker
Zeroth|ASR|Industry|docu|all|rd|0|51+ (h) / 27K (s) / 46K (u) / 181 speakers
ClovaCall|ASR|Industry|int'l|academic|no|0|80+ (h) / 60K (u) / 11K speakers
Pansori-TedXKR|ASR|Academia|int'l|academic|rd|1|3+ (h) / 3K (u) / 41 speakers
ProSem|SLU|Academia|int'l|all|rd|0|6+ (h) / 3,500 (s) / 7K (u) / 2 speakers
kosp2e|Speech translation|Industry|int'l|academic|rd|0|39K(u)
KoCHET|Other topics|Academia|int'l|academic|rd|0|NER 112K, RE 39K, ET 113K
KommonGen|Other topics||docu|all|rd|0|79K(s)
LBox Open|Other topics|Academia|int'l|academic|rd||150K
K2NLG|Other topics|Academia|int'l|academic|rd|0|4K(s)
Korean Ambiguity Data|Other topics||int'l|all|rd||35K
jejueo (JSS & JIT)|Other topics|Industry|int'l|all|rd|0|10K (JSS), 170K (JIT)
Korean GEC dataset|Other topics|Academia|int'l|academic|rd|0|155K(s pair)

## 기타 주요 데이터

|번호|데이터 종류| 데이터 설명|          
|:---:|:-----------------:|:-----------------:|
|1|[청와대 국민청원](https://www1.president.go.kr/petitions) 사이트의 [만료된 청원](https://www1.president.go.kr/petitions?only=finished) 데이터 모음| [:octocat:](https://github.com/akngs/petitions)|-|     
|2|[챗봇용 대화 응답 세트](https://github.com/songys/Chatbot_data)|챗봇용 응답 쌍과 긍부정 태깅|
|3|[영화추천시스템을 위한 데이터 세트](https://github.com/lovit/kmrd)|Synthetic dataset for recommender system created with Naver Movie rating system|
|4|[학습용 뉴스 댓글 데이터](https://www.kaggle.com/junbumlee/kcbert-pretraining-corpus-korean-news-comments)|BERT 모델과 학습에 이용한 11.62G 데이터를 모두 공개|   
|5|[AMR](https://github.com/choe-hyonsu-gabrielle/korean-amr-corpus)|[문서요약에 대한 지침](https://github.com/choe-hyonsu-gabrielle/korean-amr-guidelines)과 데이터 세트|
|6|[네이버쇼핑, Steam 플랫폼 리뷰 데이터](https://github.com/bab2min/corpus/tree/master/sentiment)|감성분석(Sentiment Analysis)을 위한 제품 별, 게임 별 별점과 후기를 수집한 데이터셋|



# 국가적 규모에서 구축한 데이터

|번호|데이터 종류| 데이터 설명|
|:---:|:-----------------:|:-----------------:|         
|1| [우리말샘](https://opendict.korean.go.kr/main)| 이 사전에 대한 설명 [:octocat:](https://github.com/songys/Dictionaries) : 다양한 어휘와 유의어 정보 등을 얻을 수 있는 대사전 : 로그인 후 전체 사전 데이터 다운로드 가능| |      
|2| [NIA 사전](https://kbig.kr/portal/kbig/knowledge/files/bigdata_report.page?bltnNo=10000000016451)|묻지도 따지지도 않고 다음 링크에서 엑셀로 다운로드 가능 |  
|3| [국립국어원 언어정보나눔터](https://ithub.korean.go.kr/user/total/database/corpusManager.do )| 로그인 후 세종2007 코퍼스나 낭독체 음성 파일 등도 다운로드 가능, 다운 받을 때 간단한 서약에 체크만 하면 되는데 자료의 크기를 작게 나누어 놓아서 여러번 체크해야 한다는 것이 단점 |  
|4| [AIHub](http://aihub.or.kr/)| 텍스트와 음성 멀티모달까지 가장 광범위한 데이터, 로그인 및 사용 목적과 기간을 명시한 사용 신청서 작성 후 허가 메일이 오면(하루 정도 걸린다) 다운로드 가능 |   

![pic](./aihub.png)

   
|번호|데이터 종류| 데이터 설명|            
|:---:|:-----------------:|:-----------------:|         
|5|[국립국어원 모두의 말뭉치](https://corpus.korean.go.kr/)| 다양한 분석 말뭉치(형태소 분석과 구문 분석 말뭉치 등), 다양한 도메인의 말뭉치(문어, 신문, 구어, 웹), 자연어 추론을 위한 말뭉치(유사 문장) 등 다양한 데이터들이 체계적으로 구축되어 있다. 로그인, 메일 인증을 거쳐 데이터를 신청할 수 있고 다운로드 받기 위해서는 연구과제명과  수행기관, 약정 기간 등이 필수 입력 요소이다. |

![pic](./everyone.png)











