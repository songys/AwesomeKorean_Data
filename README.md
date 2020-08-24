
# AwesomeKorean_Data
- 12월 15일 첫번째 버전을 만들었고 이후 박조은님의 코멘트 그리고 2020년 8월 21일 @warnikchow님의 다양한 기여와 의견을 반영하여 수정하였습니다.       
- Natural language processing의 각 분야에 대한 자료 정리는 다음 링크를 참고     [Awesome-Korean-NLP](https://github.com/datanada/Awesome-Korean-NLP) 


- 다양한 전처리 및 다운로더를 포함한 데이터 링크는 다음을 참조 [https://ratsgo.github.io/https://ratsgo.github.io/embedding/preprocess.html](https://ratsgo.github.io/embedding/preprocess.html)      


                                    
# Open Datasets
![network](./network.jpg)

- Commercially available(com), academic use only(aca), unknown(unk)
- Redistribution is possible with or without modification, if neither, or unknown (red, red/mod-x, not, unk)  
- Internationally available publication(INT) 

## 1.  Classical NLP pipeline

분석적 관점에서 원시 코퍼스로부터 형태소,(의존)구문, 의미역, 개체명, 무형대용어복원 등의 태깅을 하는 과제가 주를 이룬다. 

|No|Dataset|Typical Usage|Provider|Docu|License|Volume|Goal|Lang|Description|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|                            
|1|[KAIST Morpho-syntactically Annotated Corpus](http://semanticweb.kaist.ac.kr/home/index.php/KAIST_Corpus)|Morphological analysis|Academia|article|aca/|70M(w)| - |ko|원시코퍼스부터 다양한 코퍼스가 있다. 하나 하나의 데이터마다 Affiliation을 채워야 하지만 데이터 만드는 품을 생각하면 이 정도는 오픈 데이터로 보는 것이 좋을 듯하다.|         
|2|[Korean Tree-tagged Corpus]((http://semanticweb.kaist.ac.kr/home/index.php/KAIST_Corpus))|Tree parsing|Academia|INT|aca/red|30K(s)|-|ko|-| 
|3|[UD Korean KAIST]((http://semanticweb.kaist.ac.kr/home/index.php/KAIST_Corpus))|Dependency parsing| Academia| INT|com/red|30K (s)|-|ko|-| 
|4|[PKT-UD](https://catalog.ldc.upenn.edu/LDC2006T09)|Dependency parsing |Academia| INT| com/red|5K (s)|-|ko| 
|5|[KMOU NER](https://github.com/kmounlp/NER)| NER| Academia|article|aca/red|24K (s)|-|ko|한국어 개체명 정의 및 표지 표준화 기술보고서와 이를 기반으로 제작된 개체명 형태소 말뭉치| 
|6|[AIR x NAVER NER](http://air.changwon.ac.kr/?page_id=10)| NER |Competition| DOC |aca/not|90K (s)|-|ko|인명, 기관명, 지명 등 특정한 의미가 있다고 생각하는 명사들의 최대 범주를 태깅하는 과제에 필요한 데이터 세트| 
|7|[AIR x NAVER SLR](http://air.changwon.ac.kr/?page_id=14)|SLR|Competition|DOC|aca/not|35K(s)|-|ko|의미역 결정(Semantic Role Labeling)을 위한 데이터
| 

## 2. Entailment and sentence similarity  
실제 담화에서 어떤 문장(발화)들이 같은 의미로 기능하는 지를 실제적으로 판단하는 과제가 주를 이룬다. 단지 유사 단어나 문장 뿐만 아니라 내포하는 의미가 같은 경우 등으로 세분화해서 데이터가 구축된다.

|No|Dataset|Typical Usage|Provider|Docu|License|Volume|Goal|Lang|Description|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|                            
|1|[Question Pair](https://github.com/songys/Question_pair)| Paraphrase detection|Academia|DOC|com/red|10K (p)|-|ko| 유사 문장쌍 |            
|2|[KorNLI](https://github.com/kakaobrain/KorNLUDatasets)|NLI|Industry|INT|com/red |1,000K (p)|-|ko |자연어 이해를 위한 데이터 세트|
|3|[KorSTS](https://github.com/kakaobrain/KorNLUDatasets)|STS|Industry|INT|com/red|8,500 (p)|-|ko |자연어 이해를 위한 데이터 세트|
|4|[ParaKQC](https://github.com/warnikchow/ParaKQC)|STS|Academia|INT|com/red|540K (p)|-|ko |Parallel dataset of Korean Questions and Commands|

## 3. Semantics and question answering
자연어처리에서 '의미론'은 많은 부분에서 분류의 문제로 처리된다. 그러나 질문에 대해, 답변을 하거나, 시나 소설에서 다음에 나올 문장을 생성해 준다거나 요약문을 제공해 주는 경우도 있다. 하지만 과제 중심으로 본다면 이런 경우도 정답이 있는 것은 아닐 것이다. 좁은 범주의 고정 도메인에서 QA 문제를 풀 때는 정해진 답변을 분류 문제로 풀어서 답하게 되는 경우도 있다. 가령, 수영장 이용 안내를 챗봇으로 하는 경우 라커키 이용 방법처럼 자주 나오는 질문에 대한 답은 정해져 있는 편이 경제적일 것으로 생각된다.

|No|Dataset|Typical Usage|Provider|Docu|License|Volume|Goal|Lang|Description|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|    
|1|[NSMC](https://github.com/e9t/nsmc)|Sentiment analysis|Academia|DOC|com/red|150K / 50K (s)|-|ko|댓글을 통한 감성 분석 데이터 세트|          
|2|[BEEP!](https://www.kaggle.com/captainnemo9292/korean-extremist-website-womad-hate-speech-data)|Hate speech detection|Academia |INT |com/red |8K / 500 / 1,000 (s)|-|ko|혐오 표현 관련 데이터|                 
|3|[3i4K](https://github.com/warnikchow/3i4k)|Speech act classification |Academia |INT |com/red |55K / 6K (s)|-|ko|Intonation-aided intention identification for Korean|Structured argument extraction for Korean|    
|4|KorQuAD1|QA|Industry|INT|com/red (mod-x)|60K / 5K / 4K (p)|-|ko| 질의 응답 데이트 세트[KorQuAD 설명 동영상](https://www.youtube.com/watch?v=ntGwv6Ifoe8)|
|5|[KorQuAD2](https://korquad.github.io/)|QA|Industry|article|com/red (mod-x)|80K / 10K / 10K (p)|-|ko| -|


## 4 Parallel corpora  
병렬 코퍼스는 언어 간 연구 또는 번역 자동화를 위한 데이터 세트이다. 개인적으로는 짧은 문장에 대한 대량의 번역 데이터 세트가 있었으면 좋겠다는 바람이 있다. 지금은 신문 등의 병렬 데이터 세트가 많아서 처음 자연어처리에 입문하는 사람이 연습용으로 쓰기에는 어려움이 있다.   
|No|Dataset|Typical Usage|Provider|Docu|License|Volume|Goal|Lang|Description|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|                        
|1|[Sci-news-sum-kr](https://github.com/theeluwin/sci-news-sum-kr-50)|Summarization|Academia|DOC|aca/red|50 (p)|Eval|ko|-|네이버 뉴스 중 IT/과학 분야에서 50개에 요약 문장을 태깅한 데이터 세트|   
|2|[SAE4K](https://github.com/warnikchow/sae4k)|Summarization|Academia|INT|com/red|50K (p)|-|ko|Structured argument extraction for Korean|  
|3|[Korean Parallel Corpora](https://github.com/jungyeul/korean-parallel-corpora)|MT|Academia|INT|com/red|97K (p)|-|ko, en, fr|-|
|3|[KAIST Translation Evaluation Set2](http://semanticweb.kaist.ac.kr/home/index.php/Evaluateset2) |MT| Academia|DOC |aca/red |3K (p)|Eval|ko, en|-| 
|4|[Chinese-Korean Multilingual Corpus](http://semanticweb.kaist.ac.kr/home/index.php/Corpus9) |MT |Academia|DOC |aca/red|60K (p)|-|ko, zh |-|
|5|[Transliteration Dataset](https://github.com/muik/transliteration),  Wiktionary(https://en.wiktionary.org/wiki/Wiktionary:Main_Page) |Transliteration|Academia |DOC |com/red |35K (p)|-| ko, en |영어 단어를 한국어 표기로 변환, 위키 낱말 사전 등|-|
|6|[KAIST Transliteration Evaluation Set3](http://semanticweb.kaist.ac.kr/home/index.php/Evaluateset3)|Transliteration|Academia| DOC |aca/red|7K (p)|Eval|ko, en| 영-한 자동 음차표기를 위한 실험집합|


## 5 Korean in multilingual corpora
|No|Dataset|Typical Usage|Provider|Docu|License|Volume|Goal|Lang|Description|
|:---:|:---:|:---:|:---:|:---:|:---:|:---------:|:---------:|:---------:|:---------:|                             
|1|[Sigmorphon G2P](https://sigmorphon.github.io/sharedtasks/2020/task1/) |G2P conversion|Competition |DOC |unk/unk |3,600 / 450 / 450 (p) |-|ko, en, hy, bg, fr, ka, hi, hu, is, lt, el|Multilingual Grapheme-to-Phoneme Conversion|-|
|2|[PAWS-X](https://github.com/google-research-datasets/paws/tree/master/pawsx) | Paraphrase detection |Industry|INT |com/red |5K / 2K / 2K (p)|-|ko, fr, es, de, zh, ja|-| 
|3|[TyDi-QA](https://github.com/google-research-datasets/tydiqa)|QA|Industry|INT [DOC](https://arxiv.org/abs/2003.05002)|com/red |11K / 1,698 / 1,722 (p)|-|ko, en, ar, bn, fi, ja, id, sw, ru, te, th |-|
|4|[XPersona](https://github.com/HLTCHKUST/Xpersona) |Dialog |Academia |INT [Doc](https://arxiv.org/abs/2003.07568) |com/red |299 (d)|- |ko, en, it, fr, id, zh, ja / 4,684 (s)| -|        


## 6. Speech recognition and spoken language understanding
|No|Dataset|Typical Usage|Provider|Docu|License|Volume|Goal|Lang|Description|
|:---:|:---:|:---:|:---:|:---:|:---:|:---------:|:---------:|:---:|:---:|
|1|[KSS](https://github.com/Kyubyong/kss) |ASR|Academia|DOC|aca/red|12+ (h)/ 13K (u) / 1 speaker |-|ko |STT|    |2|[Zeroth](https://github.com/goodatlas/zeroth) |    ASR |Industry |DOC|com/red|51+(h)/ 27K (s)/ 46K (u)/181 speakers|-|ko|-|          
|3|[ClovaCall](https://github.com/clovaai/ClovaCall)|ASR|Industry|INT|aca/not|80+ (h)/ 60K (u)/ 11K speakers|-|ko|-|         
|4|[Pansori-TedXKR](https://github.com/yc9701/pansori-tedxkr-corpus)|ASR|Aca|INT|aca/red (mod-x)|3+ (h)/ 3K (u)/ 41 speakers|-|ko|-|           
|5|[ProSem](https://github.com/warnikchow/prosem)|SLU|Aca|INT|com/red|6+ (h) / 3,500 (s) /7K (u)/2 speakers|-|ko|-|          



## 7. 시사 데이터

|번호|데이터 종류| 데이터 설명|          
|:---:|:-----------------:|:-----------------:|
|1.|[한국 정치인 뉴스 데이터 세트](https://github.com/lovit/politician_news_dataset)|-|
|2|[청와대 국민청원](https://www1.president.go.kr/petitions) 사이트의 [만료된 청원](https://www1.president.go.kr/petitions?only=finished) 데이터 모음| [:octocat:](https://github.com/akngs/petitions)|-|
|3|[공공데이터포털 뉴스빅데이터](https://www.data.go.kr/dataset/15012945/fileData.do) |뉴스 데이터 'Kinds' 기반 분석 자료, 기사 메타 제공|

## 8. 기타 데이터
|번호|데이터 종류| 데이터 설명|          
|:---:|:-----------------:|:-----------------:|
|1|[챗봇용 대화 응답 세트](https://github.com/songys/Chatbot_data)|-|
|2|[영화추천시스템을 위한 데이터 세트](https://github.com/lovit/kmrd)|Synthetic dataset for recommender system created with Naver Movie rating system|


# 국가적 규모에서 구축한 데이터

|번호|데이터 종류| 데이터 설명|
|:---:|:-----------------:|:-----------------:|         
|1| [우리말샘](https://opendict.korean.go.kr/main)| 이 사전에 대한 설명 [:octocat:](https://github.com/songys/Dictionaries) : 다양한 어휘와 유의어 정보 등을 얻을 수 있는 대사전 : 로그인 후 전체 사전 데이터 다운로드 가능| |      
|2| [NIA 사전](https://kbig.kr/portal/kbig/knowledge/files/bigdata_report.page?bltnNo=10000000016451)|묻지도 따지지도 않고 다음 링크에서 엑셀로 다운로드 가능 |    
|3| [AIHub](http://aihub.or.kr/)| 텍스트와 음성 멀티모달까지 가장 광범위한 데이터, 로그인 및 사용 목적과 기간을 명시한 사용 신청서 작성 후 허가 메일이 오면(하루 정도 걸린다) 다운로드 가능 |                     
|4| [국립국어원 언어정보나눔터](https://ithub.korean.go.kr/user/total/database/corpusManager.do )| 로그인 후 세종2007 말뭉치나 낭독체 음성 파일 등도 다운로드 가능, 다운 받을 때 간단한 서약에 체크만 하면 되는데 자료의 크기를 작게 나누어 놓아서 여러번 체크해야 한다는 것이 단점 |    
|5|[국립국어원 모두의 말뭉치](https://corpus.korean.go.kr/)| 다양한 분석 말뭉치(형태소 분석과 구문 분석 말뭉치 등), 다양한 도메인의 말뭉치(문어, 신문, 구어, 웹), 자연어 추론을 위한 말뭉치(유사 문장) 등 다양한 데이터들이 체계적으로 구축되어 있다. 로그인, 메일 인증을 거쳐 데이터를 신청할 수 있고 다운로드 받기 위해서는 연구과제명과  수행기관, 약정 기간 등이 필수 입력 요소이다. |






