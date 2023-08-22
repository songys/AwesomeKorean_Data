
# AwesomeKorean_Data

- 비교적 대부분의 사람들이 접근할 수 있는 오픈 데이터를 정리하였다. 구할 수 있는 모든 데이터를 쏟아 부어서 end to end로 모델을 만들어 보겠다는 포부를 가진 분들의 진입을 쉽게하기 위한 목적이고, 정교한 데이터 구축을 위해서는 이후에 어떠한 데이터가 필요한지를 살펴보기 위한 과정이다.            

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
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|[KLUE](https://klue-benchmark.com/)|인공지능의 언어 능력 평가|Industry|int'l|all|rd|0|DP - 15K (s), DST - 10K (d), MRC - 29K (p), NER - 31K (s), NLI - 30K (p), RE - 48K (s), STS - 13K (p), TC - 64K (s) |
|[KoBEST](https://huggingface.co/datasets/skt/kobest_v1)|인공지능의 언어 능력 평가|Industry|int'l|all|rd|0|BoolQ - 6K (p), COPA - 5K (s), KB-WiC - 6K (s), KB-HellaSwag - 3K (p & s), SentiNeg - 4K (s)|
|[KAIST Morpho-Syntactically Annotated Corpus](http://semanticweb.kaist.ac.kr/home/index.php/KAIST_Corpus)|형태분석|Academia|paper|academic|no|0|70M (w)|
|[OpenKorPOS](https://github.com/openkorpos/openkorpos)|형태분석|Academia|int'l|all|rd|0|55M(w)|
|[KAIST Korean Tree-Tagging Corpus](http://semanticweb.kaist.ac.kr/home/index.php/KAIST_Corpus)|구문분석|Academia|int'l|academic|no|0|30K (s)|
|[UD Korean KAIST](https://github.com/emorynlp/ud-korean)|의존구문분석|Academia|int'l|academic|no|1|27K (s)|
|[PKT-UD](https://github.com/emorynlp/ud-korean)|의존구문분석|Academia|int'l|academic|no|0|5K (s)|
|[KMOU NER](https://github.com/kmounlp/NER)|개체명|Academia|paper|academic|rd|0|24K (s)|
|[AIR x NAVER NER](http://air.changwon.ac.kr/?page_id=10)|개체명|Competition|docu|academic|no|0|90K (s)|
|[AIR x NAVER SRL](http://air.changwon.ac.kr/?page_id=14)|의미역 결정|Competition|docu|academic|no|0|35K (s)|
|[KoNEC & KoNNEC](https://github.com/korean-named-entity/konne)|개체명|Academia|docu|academic|no|0|26K(s)|
|[Question Pair](https://github.com/songys/Question_pair)|유사문장쌍에 대한 구분|Academia|docu|all|rd|0|10K (p)|
|[KorNLI](https://github.com/kakaobrain/kor-nlu-datasets)|자연어추론|Industry|int'l|all|rd|0|1,000K (p)|
|[KorSTS](https://github.com/kakaobrain/kor-nlu-datasets)|유사문장 분석|Industry|int'l|all|rd|0|8,500K (p)|
|[ParaKQC](https://github.com/warnikchow/ParaKQC)|유사문장 분석|Academia|int'l|all|rd|0|540K (p)|
|[StyleKQC](https://paperswithcode.com/dataset/stylekqc)|유사문장판별|Academia|int'l|all|rd|0|30K(s)|
|[Korean Smile Style Dataset](https://github.com/smilegate-ai/korean_smile_style_dataset)|유사문장판별|Industry|docu|academic|rd|0|2,5K(d)|
|[NSMC](https://github.com/e9t/nsmc)|감성분석|Academia|docu|all|rd|0|150K / 50K (s)|
|[Kocasm](https://github.com/SpellOnYou/korean-sarcasm)|감성분석|Academia|docu|all|rd|0|9K (s)|
|[BEEP!](https://github.com/kocohub/korean-hate-speech)|혐오표현탐지|Academia|int'l|all|rd|0|8K / 0.5K / 1K (s)|
|[APEACH](https://github.com/jason9693/APEACH)|혐오표현탐지|Academia|int'l|all|rd|0|4K|
|[Unsmile](https://github.com/smilegate-ai/korean_unsmile_dataset)|혐오표현탐지|Industry|docu|academic|rd|0|19K|
|[HateScore](https://github.com/sgunderscore/hatescore-korean-hate-speech)|혐오표현탐지|Academia|int'l|academic|rd|1|35K|
|[KOLD](https://github.com/boychaboy/KOLD)|혐오표현탐지|Academia|int'l|all|rd|0|40K|
|[DKTC](https://github.com/tunib-ai/DKTC)|혐오표현탐지|Industry|docu|academic|rd|0|1.5K|
|[K-MHaS](https://github.com/adlnlp/K-MHaS)|혐오표현탐지|Academia|int'l|all|rd|0|109K|
|[3i4K](https://github.com/warnikchow/3i4k)|화행분석|Academia|int'l|all|rd|0|55K / 6K (s)|
|[KorQuAD 1.0](https://korquad.github.io/)|질의응답|Industry|int'l|all|rd|1|60K / 5K / 4K (p)|
|[KorQuAD 2.0](https://korquad.github.io/)|질의응답|Industry|paper|all|rd|1|80K / 10K / 10K (p)|
|[HuLiC](https://github.com/smilegate-ai/HuLiC)|대화|Industry|docu|academic|rd|0|115K|
|[OPELA](https://github.com/smilegate-ai/OPELA/blob/main/OPELA_Kor_Ver.md)|대화|Industry|int'l|academic|rd|0|560K (d)|
|[Sci-news-sum-kr](https://github.com/theeluwin/sci-news-sum-kr-50)|요약|Academia|docu|academic|rd|0|50K (p)|
|[sae4K](https://github.com/warnikchow/sae4k)|요약|Academia|int'l|all|rd|0|50K (p)|
|[Korean Parallel Corpora](https://github.com/jungyeul/korean-parallel-corpora)|기계번역|Academia|int'l|all|rd|1|100K (p)|
|[KAIST Translation Evaluation Set](http://semanticweb.kaist.ac.kr/home/index.php/Evaluateset2)|기계번역|Academia|docu|academic|no|0|3K (p)|
|[KAIST Chinese-Korean Multilingual Corpus](http://semanticweb.kaist.ac.kr/home/index.php/Corpus9)|기계번역|Academia|docu|academic|no|0|60K (p)|
|[Transliteration Dataset](https://github.com/muik/transliteration)|영한기계번역|Academia|docu|all|rd|0|35K (p)|
|[KAIST Transliteration Evaluation Set](http://semanticweb.kaist.ac.kr/home/index.php/Evaluateset3)|기계번역|Academia|docu|academic|no|0|7K (p)|
|[SIGMORPHON G2P](https://sigmorphon.github.io/sharedtasks/2020/task1/)|다중언어의 자소를 음소로 변환|Competition|int'l|all|rd|0|3.6K/ 0.45K / 0.45K (p)|
|[PAWS-X](https://github.com/google-research-datasets/paws/tree/master/pawsx)|유사문장판별|Industry|int'l|all|rd|0|5K / 2K / 2K (p)|
|[TyDi-QA](https://github.com/google-research-datasets/tydiqa)|질의응답|Industry|int'l|all|rd|0|11K / 1,7K / 1,7K(p)|
|[XPersona](https://github.com/HLTCHKUST/Xpersona)|다중언어 대화|Academia|int'l|all|rd|0|0.3K(d) / 4.7K (s)|
|[CareCall](https://github.com/naver-ai/carecall-memory)|대화|Industry|int'l|academic|rd|0|10K|
|[MultiCoNER](https://multiconer.github.io/multiconer_1/dataset)|개체명|Competition|int'l|all|rd|0|178K / 2.6K (s)|
|[Multilingual Tweet Intimacy Analysis](https://arxiv.org/abs/2210.01108)|감성분석|Competition|int'l|unk|unk|0|2K(instances)|
|[IWSLT 2023](https://github.com/kevinduh/iwslt22-dialect)|기계번역|Competition|int'l|all|rd|0|3K (p)|
|[KSS](https://github.com/Kyubyong/kss)|한국어 1인 발화|Academia|docu|academic|rd|0|12+ (h) / 13K (u) / 1 speaker|
|[Zeroth](https://github.com/goodatlas/zeroth)|Kaldi 기반의 음성 인식(ASR)|Industry|docu|all|rd|0|51+ (h) / 27K (s) / 46K (u) / 181 speakers|
|[ClovaCall](https://github.com/clovaai/ClovaCall)|음성인식|Industry|int'l|academic|no|0|80+ (h) / 60K (u) / 11K speakers|
|[pansori-tedxkr-corpus](https://github.com/yc9701/pansori-tedxkr-corpus)|음성인식|Academia|int'l|academic|rd|1|3+ (h) / 3K (u) / 41 speakers|
|[ProSem](https://github.com/warnikchow/prosem)|의미를 구별하는 운율 요소(SLU)|Academia|int'l|all|rd|0|6+ (h) / 3,500 (s) / 7K (u) / 2 speakers|
|[kosp2e](https://github.com/warnikchow/kosp2e)|한국어 대화의 영어 번역|Industry|int'l|academic|rd|0|39K(u)|
|[KoCHET]([https://github.com/Gyeongmin47/KoCHET-A-Korean-Cultural-Heritage-corpus-for-Entity-related-Tasks)|역사자료|Academia|int'l|academic|rd|0|NER 112K, RE 39K, ET 113K|
|[KommonGen](https://github.com/nlpai-lab/KommonGen)|문장 생성을 위한 개념집합세트||docu|all|rd|0|79K(s)|
|[LBox Open](https://github.com/lbox-kr/lbox-open)|판결문|Academia|int'l|academic|rd||150K|
|[K2NLG](https://github.com/machinereading/K2NLG-Dataset)|기계독해|Academia|int'l|academic|rd|0|4K(s)|
|[Korean Ambiguity Data](https://github.com/bareun-nlp/korean-ambiguity-data)|모호한문장판별||int'l|all|rd||35K|
|[jejueo](https://github.com/kakaobrain/jejueo)|제주어|Industry|int'l|all|rd|0|10K (JSS), 170K (JIT)|
|[Korean GEC dataset](https://github.com/soyoung97/Standard_Korean_GEC)|맞춤법오류|Academia|int'l|academic|rd|0|155K(s pair)|

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


   
|번호|데이터 종류| 데이터 설명|            
|:---:|:-----------------:|:-----------------:|         
|5|[국립국어원 모두의 말뭉치](https://corpus.korean.go.kr/)| 다양한 분석 말뭉치(형태소 분석과 구문 분석 말뭉치 등), 다양한 도메인의 말뭉치(문어, 신문, 구어, 웹), 자연어 추론을 위한 말뭉치(유사 문장) 등 다양한 데이터들이 체계적으로 구축되어 있다. 로그인, 메일 인증을 거쳐 데이터를 신청할 수 있고 다운로드 받기 위해서는 연구과제명과  수행기관, 약정 기간 등이 필수 입력 요소이다. |

|말뭉치 이름|발행기관	발행연도|원시말뭉치(raw) VS 주석이 있는 말뭉치(tagged)|예|분량|공개범위|	비고|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|일상대화|모두의말뭉치	2020 (버전 1.0)|raw|	반려동물을 키우고 계신가요|	파일 2,232개, 총 317MB|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)| - |  
|어휘의미분석|모두의말뭉치	2020 (버전 1.0)|tagged|"""word"": ""제주"", ""sense_id"": 8, ""pos"": ""NNP"", ""begin"": 1, ""end"": 3, ""word_id"": 1"	|2019년도에 구축된 300만 어절 규모(문어 200만, 구어 100만 어절)와 메신저 대화 말뭉치 (92만 어절)를 대상으로 형태 분석과 어휘 의미(체언류와 용언류)를 분석한 말뭉치|	국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)| - |
|어휘관계|	모두의말뭉치	2020 (버전 1.0)|tagged|	가가대소 방소 유의어	|우리말샘 사전 기반 어휘 관계 기초 자료 20만 쌍(비슷한말 60,000쌍, 반대말 10,000쌍, 상위어 70,000쌍, 하위어 60,000쌍|	국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)| - |
|문법성판단|	모두의말뭉치	2020 (버전 1.0)|tagged|"높은 달이 떴다. 4.981(mean) |달이 뜸이 높았다. 2.223(mean)|	총 19,940개 문장(문법적 문장 9,970개 문장, 비문법적 문장,  파일 4개, 총 3.19MB |국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)| - |     
|개체명|	모두의말뭉치	2020 (버전 1.0)|tagged|	"""form"": ""멕시코"",""label"": ""LC""" |	총 300만 어절(문어 200만 어절, 구어 100만 어절), 파일 2개, 총 909MB|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)| - |
|유사문장|모두의말뭉치	2020 (버전 1.0)|tagged|	"경기 성남시 판교신도시에서 이달 분양하는 중대형 아파트의 3.3m²당 분양가가 1500만 원 후반대로 결정될 것으로 보이는데 이는 2006년보다 200만 원 정도 싼 가격이다.|	179,589개 문장,  파일 1개, 총 42.5MB	|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)|	인간이 생성한 문장과 기계가 생성한 문장 쌍의 유사도| 
|웹|모두의말뭉치	2020 (버전 1.0)|raw| """title"": ""비타민 사기 진짜 어려워.."", ""form"": ""오메가3와 비타민C, 달맞이꽃종자유 등을 사려고 몇 시간을 검색하며 공부했다. 그 결과 오염되지 않은 바다에서 잡힌 먹이사슬의 하단에 있는 생선이 좋다고 들었는데(중략)|블로그 11,521건 게시판 9,089건 누리 소통망 1,989,656건 -리뷰: 96,810건|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)|2023년 8월 검색 결과에서는 모두의 말뭉치 홈페이지에 없음|
|신문|모두의말뭉치	2020 (버전 1.0)|raw|2008년의 마지막 새벽, 언론의 카메라는 서울 여의도를 향했다. 방송법 등 주요 쟁점 법안이 상정될 국회 본회의장을 두고 여야 의원들의 전쟁을 기다리고 있었던 것| 기사 3,536,491건(2009년부터 2018년까지 10년 동안 생산된 신문 기사 연 1억여 어절),  파일 363개, 총 15.6GB	| 국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며(=학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)|(버전 1.0) 2020. 8. 25. (버전 2.0) 2021. 3. 30. - 기사 추가|
|문어	|모두의말뭉치	2020 (버전 1.0)|raw|01범보다 무서운 곶감|책, 잡지, 보고서 등 저작권 문제가 해결된 저작물 10,045종의 문어 원시 말뭉치, 파일 10,045개, 총 4.24GB	|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)	|버전에 따라 분량에 차이가 날 수 있음(저작권 미해결 자료 배포 시기에 차이가 있음|
|구어|모두의말뭉치	2020 (버전 1.0)|raw	|title: EBS 정오뉴스 2018년 1월, topic: 도서관의 변신, 메이커 스페이스에 대한 기사, form: 미국의 공공도서관들이 새로운 모습으로 변신하고 있습다.|공적 독백 2,490건 공적 대화 19,104건, 준구어-대본 4,102건(드라마 ), 파일 25,696개, 총 6.73GB	|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)| - |    
|문서요약|	모두의말뭉치	2020 (버전 1.0)|tagged|-|기사 제목, 부제목-1문장, 기사, 기사 요약-2문장 이상	신문 말뭉치에서 추출한 기사 4,389건이 대상 말뭉치에서 기사 추출 주제 및 요약 작성 문장 13,167개|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)| - |
|구문|모두의말뭉치	2020 (버전 1.0)	|tagged|	"""word_form"": ""판교신도시에서"", ""head"": 5, ""label"": ""NP_AJT"""	"총 300만 어절 문어 200만 어절, 구어 200만 어절, 문어 1.07GB, 구어 583MB"	|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)	| - |
|형태분석|모두의말뭉치	2020 (버전 1.0)|tagged|"""form"": ""제주"", ""label"": ""NNP"""|	300만 어절(문어 200만 어절, 구어 100만 어절) 파일 2개, 총 2.31GB	|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)	| - |
|추론확신성	|모두의말뭉치	2020 |tagged|"변화에 대한 적응이 항상 성공적일 수는 없다. 당신을 힘들게 하는 팀원이 당신의 리더십을 키우는 원동력임을 기억한다면, 갈등을 겪을 때마다 당신은 더욱 발전할 수 있는 기회를 "|신문, 준구어 말뭉치에서 대상 담화 추출, 파일 1개, 총 272KB	|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)	| - |
|일상대화|모두의말뭉치	2021|	raw|아 지금|	파일 4,143개, 총 560MB|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)|  - |    
|신문|모두의말뭉치	2021|	raw	|대통령, 시장 방문만 하지 말고 실천해달라	|2020년 생산된 신문 기사 729,280건, 파일 35개, 총 2.95GB |국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)	| - |  
|국회회의록|모두의말뭉치	2021|	raw|	회의를 시작하도록 하겠습니다.|5,395건(73,478,080어절), : 파일 5,395개, 총 307MB	|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)	| - |
|추론확신성|모두의말뭉치	2021|tagged|"P1: 네. P5: 술을 많이 마셔도 회복이 될겁니다. 옥희 선생님 같은 경우에도 P4: 네네 P5: 소시적에는 밤 새워서 이제 나이트에서 놀고 그러셔도 금방 회복이 되셨죠. P3: 아니나 놀다니요. P3: 일하러 가죠. P5: 아~ 일을하셨구나. P5: 예. P3: 예. P5:	|문어, 신문, 구어, 대화, 파일 1개, 총 1.457KB|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)	| - |     
|온라인대화| 모두의말뭉치	2022|raw|"지금 운동하러가려고하는데 반팔 반바지 입으니까 선크림을 발라야돼	|총 74,665건(대화 메시지,  파일 47,421개, 총 835MB | 국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)	|카카오톡기반 2인 대화 및 다자간 대화 |
|신문|모두의말뭉치	2022	|raw|	변이 바이러스’ 잡는 모더나 백신 2000만명 올 2분기 한국 온다.|2021년 생산된 신문 기사 978,342건, 파일 34개(zip 압축파일 1개, 898MB)|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)| - |
|메신저|	모두의말뭉치 2022|	raw	|짜쟌|총 3,836건(대화 메시지 691,535개), 총 212MB	|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)|친구 사이에 사용하는 비속어 등이 일부 남아 있음|
|맞춤법교정|	모두의말뭉치	2022|	tagged|	하이하이	|약 400만 어절, 파일 1개, 총 517MB	|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)|메신저 말뭉치에 남아 있는 비속어 등도 수정한 말뭉치|
|개체명연결|	모두의말뭉치	2022	|tagged|	"""id"": 2, ""form"": ""고대"", ""label"": ""DT_DYNASTY"", ""begin"": 27, ""end"": 29, ""kid"": ""07070000000019"", ""wikiid"": ""378315"", ""URL"": ""https://ko.wikipedia.org/wiki/%EA%B3%A0%EC%A0%84_%EA%B3%A0%EB%8C%80"	" |총 약 1,100만 어절(웹 500만, 문어 300만, 구어 300만 어절)| - 국립국어원 개체명 분석 말뭉치 2020(버전 2.1): 500만 어절(웹) - 국립국어원 개체명 분석 말뭉치 2021(버전 1.0): 600만 어절(문어 300만, 구어 300만 어절), 파일 323개, 총 255MB"	|국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며( =학습에 사용할 수 있음, 재배포금지) 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요(=사전 승인 및 출판후 알림)| - |
|논문자료요약|NIA_AIHUB	2021	|raw|배경: 현재 대변검경검사에서는 적절한 정도관리물질이 없어 질관리가 미진한 실정이다.| 	학술논문 18만 건에서 전체(생성) 요약 18만 건, 섹션별 (생성)요약 18만 건, 특허명세서 전체 (생성)요약 17만 건, 섹션별 (생성) 요약 17만 건 등 총 70만 건의 요약문 도출, 1.64 GB|	학습 가능, 재업로드 금지	|  - |
|대규모구매도서기반한국어|NIA_AIHUB	2021|	raw|	대지에 뿌리를 내리고사는 식물이 보기에 인간은 바람결에 이리저리 휘몰아 다니는 존재이다.	|16.86 GB	|학습 가능, 재업로드 금지	|책의 문장 순서대로 정렬되어 있지 않음(확인 필요)| - |
