
# AwesomeKorean_Data

- 비교적 대부분의 사람들이 접근할 수 있는 오픈 데이터를 정리하였다. 구할 수 있는 모든 데이터를 쏟아 부어서 end to end로 모델을 만들어 보겠다는 포부를 가진 분들의 진입을 쉽게하기 위한 목적이고, 정교한 데이터 구축을 위해서는 이후에 어떠한 데이터가 필요한지를 살펴보기 위한 과정이다.            

- 12월 15일 첫번째 버전을 만들었고 이후 박조은님의 코멘트 그리고 2020년 8월 21일 @warnikchow님의 다양한 기여와 의견을 반영하여 수정하였고 2020년 10월 18일 [메인 레포](https://github.com/ko-nlp/Open-korean-corpora)를 이동하였다. 메인 레포와 함께 데이터 링크와 약간의 설명을 보강하여 운영 중이다.   


- Natural language processing의 각 분야에 대한 자료 정리는 다음 링크를 참고     [Awesome-Korean-NLP](https://github.com/datanada/Awesome-Korean-NLP)   


- 다양한 전처리 및 다운로더를 포함한 데이터 링크는 다음을 참조 [https://ratsgo.github.io/embedding/preprocess.html](https://ratsgo.github.io/embedding/preprocess.html)      

- 코퍼스 패키지에 많은 관심이 필요합니다! 웹에 공개되어 있는 한국어 텍스트 데이터들을 손쉽게 로딩하고, 이를 이용하여 모델링한 후 evaluation 까지 편하게 수행하는 / 즉 한국어 텍스트 데이터를 위한 huggingface.nlp 작업 중인 페이지는 다음을 참조, [ko-nlp](https://github.com/ko-nlp/Korpora)

- 24년 10월 9일 한글날 기준 허깅페이스에서 2번 이상 다운받은 데이터를 다음 링크 참조 https://github.com/songys/huggingface_KoreanDataset
                                    
# Open Datasets
![network](./network.jpg)

- Commercially available(com), academic use only(Academia), unknown(unk)
- Redistribution is possible with or without modification, if neither, or unknown (rd, rd/mod-x, no, unk)  
- Internationally available publication(inter) 


아래 목록은 [Open-korean-corpora](https://github.com/ko-nlp/Open-korean-corpora)의 2026년 6월 업데이트 기준을 따라 나누었다. 각 표의 열은 `Dataset`, `Typical Usage`, `Provider`, `Docu.`, `License`, `Redist`, `mod-x`, `Volume` 순서이다.

### 2026년 6월 업데이트에서 새로 추가한 데이터셋 (2020–2025)

이번 업데이트에서는 2020년부터 2025년까지 공개된 데이터셋을 분야별로 추가하였다.

- Benchmark studies: Open-Ko-LLM, HAE-RAE Bench, KMMLU, KULTURE Bench, KMMLU-Redux/Pro, KoBALT
- Intention and sentiment: KMRE, ToM-Diary, KEmoFact, KPC-cF, KoCoSa, KOTE, CARBD-Ko, KPoEM
- Offensive language, fairness and bias (추가된 분야): KoMultiText, K-HATERS, KoSBi, SQuARe, KoBBQ, KCDD, LifeTox
- QA and dialogue: KorWikiTQ, CLIcK, KoDialogBench, KorNAT, K-MMBench, K-Viscuit, KoSimpleQA, KoPIQA
- Summarization, translation, transliteration: OPUS-MT ko-en, Naver News Summary, KoreaScience Summary, SSL, KPC, KNOTICED
- Korean in multilingual corpora: XL-Sum, MASSIVE
- Speech corpora: OLKAVS, KMSAV
- Other topics: KorMedMCQA, KBMC, ESG-Kor, KBL, FunctionChat-Bench, KCL, KorMedLawQA

연도별 수록 데이터셋 수는 다음과 같다 (총 100개).

|연도|2015|2016|2018|2019|2020|2021|2022|2023|2024|2025|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|데이터셋 수|1|3|8|7|11|5|21|10|25|9|

## 1. Benchmark studies

|Dataset|Typical Usage|Provider|Docu.|License|Redist|mod-x|Volume|
|:---|:---|:---:|:---:|:---:|:---:|:---:|:---|
|[KLUE](https://klue-benchmark.com/)|Benchmark studies|Industry|int'l|all|rd|0|DP - 15K (s), DST - 10K (d), MRC - 29K (p), NER - 31K (s), NLI - 31K (p), RE - 48K (s), STS - 12K (p), TC - 63K (s)|
|[KoBEST](https://huggingface.co/datasets/skt/kobest_v1)|Benchmark studies|Industry|int'l|all|rd|0|BoolQ - 5.8K (p), COPA - 4.6K, KB-WiC - 5.2K (p), KB-HellaSwag - 3K, SentiNeg - 4.8K|
|[Ko-H5/Open-Ko-LLM](https://huggingface.co/spaces/upstage/open-ko-llm-leaderboard)|LLM benchmark|Industry|int'l|all|rd|0|Ko-ARC, Ko-HellaSwag, Ko-MMLU, Ko-TruthfulQA, Ko-CommonGen v2; Season 2 tasks|
|[HAE-RAE Bench](https://huggingface.co/datasets/HAERAE-HUB/HAE_RAE_BENCH_1.1)|LLM benchmark|Academia|int'l|all|rd|0|1.5K questions, 6 tasks|
|[KMMLU](https://huggingface.co/datasets/HAERAE-HUB/KMMLU)|LLM benchmark|Academia|int'l|all|rd|0|35K MCQs, 45 subjects|
|[KULTURE Bench](https://github.com/wangxiaonan-git/KULTUREBench)|Cultural benchmark|Academia|int'l|academic|unk|0|-|
|[KMMLU-Redux](https://huggingface.co/datasets/LGAI-EXAONE/KMMLU-Redux) / [KMMLU-Pro](https://huggingface.co/datasets/LGAI-EXAONE/KMMLU-Pro)|LLM benchmark|Industry|int'l|all|rd|1|2.6K / 2.8K problems|
|[KoBALT](https://huggingface.co/datasets/snunlp/KoBALT-700)|Linguistic benchmark|Academia|int'l|academic|rd|1|700 MCQs|
## 2. Parsing and tagging

|Dataset|Typical Usage|Provider|Docu.|License|Redist|mod-x|Volume|
|:---|:---|:---:|:---:|:---:|:---:|:---:|:---|
|[UD Korean KAIST](https://github.com/emorynlp/ud-korean)|Dependency parsing|Academia|int'l|academic|none|0|27K (s)|
|[PKT-UD](https://github.com/emorynlp/ud-korean)|Dependency parsing|Academia|int'l|academic|none|0|5K (s)|
|[AIR x NAVER NER/SRL](https://github.com/naver/nlp-challenge)|NER, SRL|Competition|dom.|academic|none|0|NER - 90K (s), SRL - 35K (s)|
|[KMOU NER](https://github.com/kmounlp/NER)|NER|Academia|dom.|academic|rd|0|24K (s)|
|[OpenKorPOS](https://github.com/openkorpos)|POS tagging|Academia|int'l|all|rd|0|55M (w)|
|[KoNEC & KoNNEC](https://github.com/korean-named-entity/konne)|NER|Academia|dom.|all|rd|0|26K (s)|
## 3. Entailment, sentence similarity, and paraphrase

|Dataset|Typical Usage|Provider|Docu.|License|Redist|mod-x|Volume|
|:---|:---|:---:|:---:|:---:|:---:|:---:|:---|
|[Question Pair](https://github.com/songys/Question_pair)|Paraphrase detection|Academia|dom.|all|rd|0|10K (p)|
|Korean PPDB|Paraphrase database|Academia|int'l|unk|unk|0|-|
|[KorNLI/KorSTS](https://github.com/kakaobrain/KorNLUDatasets)|NLI, STS|Industry|int'l|all|rd|0|KorNLI - 940K train (p), KorSTS - 5.7K train (p)|
|[ParaKQC](https://github.com/warnikchow/ParaKQC)|Paraphrase detection|Academia|int'l|all|rd|0|540K (p)|
|[StyleKQC](https://github.com/cynthia/stylekqc)|Style transfer, paraphrase detection|Academia|int'l|all|rd|0|30K (s)|
|[Korean Smile Style Dataset](https://github.com/smilegate-ai/korean_smile_style_dataset)|Style transfer|Industry|dom.|academic|rd|0|2.5K (d)|
|[KoSEnd](https://github.com/seungukyu/KoSEnd)|Linguistic evaluation|Academia|int'l|academic|unk|0|-|
## 4. Intention understanding and sentiment analysis

|Dataset|Typical Usage|Provider|Docu.|License|Redist|mod-x|Volume|
|:---|:---|:---:|:---:|:---:|:---:|:---:|:---|
|[NSMC](https://github.com/e9t/nsmc)|Sentiment analysis|Academia|int'l|all|rd|0|200K (s)|
|[3i4K](https://github.com/warnikchow/3i4k)|Speech act classification|Academia|int'l|all|rd|0|61K (s)|
|[Kocasm](https://github.com/SpellOnYou/korean-sarcasm)|Sarcasm detection|Academia|dom.|all|rd|0|9K (s)|
|[KMRE](https://github.com/passing2961/KMRE)|Emotion classification|Academia|int'l|all|rd|0|-|
|[ToM-Diary](https://github.com/humanfactorspsych/covid19-tom-empathy-diary)|Theory of mind analysis|Academia|dom.|academic|rd|1|18K diaries, 74K (s)|
|[KEmoFact](https://www.nature.com/articles/s41598-023-45992-8)|Emotion factor extraction|Academia|int'l|unk|unk|0|-|
|[KPC-cF](https://anonymous.4open.science/r/KPC-cF-21E8)|Aspect-based sentiment classification|Academia|int'l|academic|rd|0|Kor-SemEval, KR3|
|[KoCoSa](https://github.com/Yu-billie/KoCoSa_sarcasm_detection)|Sarcasm detection|Academia|int'l|all|rd|0|12.8K (d)|
|[KOTE](https://github.com/searle-j/KOTE)|Emotion classification|Academia|int'l|academic|rd|1|50K comments, 250K annotations|
|[CARBD-Ko](https://arxiv.org/abs/2402.15046)|Aspect-based sentiment classification|Academia|int'l|academic|unk|0|-|
|[KPoEM](https://github.com/AKS-DHLAB/KPoEM)|Emotion detection|Academia|int'l|all|rd|0|-|
## 5. Offensive language detection, fairness and bias

|Dataset|Typical Usage|Provider|Docu.|License|Redist|mod-x|Volume|
|:---|:---|:---:|:---:|:---:|:---:|:---:|:---|
|[BEEP!](https://github.com/kocohub/korean-hate-speech)|Hate speech detection|Academia|int'l|all|rd|0|9.4K (s)|
|[APEACH](https://github.com/jason9693/APEACH)|Hate speech detection|Academia|int'l|all|rd|0|4K (s)|
|[Korean Unsmile Dataset](https://github.com/smilegate-ai/korean_unsmile_dataset)|Hate speech detection|Industry|dom.|academic|rd|1|19K (s)|
|[HateScore](https://github.com/sgunderscore/hatescore-korean-hate-speech)|Hate speech detection|Academia|int'l|academic|rd|0|35K (s)|
|[KOLD](https://github.com/boychaboy/KOLD)|Offensive language detection|Academia|int'l|all|rd|0|40K (s)|
|[K-MHaS](https://github.com/adlnlp/K-MHaS)|Hate speech detection|Academia|int'l|all|rd|0|109K (s)|
|[DKTC](https://github.com/tunib-ai/DKTC)|Threatening conversation detection|Industry|dom.|academic|rd|0|4.5K (d)|
|[KODOLI](https://github.com/cardy20/KODOLI)|Offensive language detection|Academia|int'l|all|rd|0|38K (s)|
|[KoMultiText](https://github.com/Dasol-Choi/KoMultiText)|Bias and profanity detection|Academia|int'l|all|rd|0|150K comments|
|[K-HATERS](https://github.com/ssu-humane/K-HATERS)|Offensive language detection|Academia|int'l|all|rd|0|192K comments|
|[KoSBi](https://github.com/naver-ai/korean-safety-benchmarks)|Social bias detection|Industry|int'l|all|rd|0|34K (p)|
|[SQuARe](https://github.com/naver-ai/korean-safety-benchmarks)|Safe response generation|Industry|int'l|all|rd|0|49K questions, 88K responses|
|[KoBBQ](https://github.com/naver-ai/KoBBQ)|Bias benchmark|Industry|int'l|all|rd|0|76K samples|
|[KCDD](https://sites.google.com/view/kcdd)|Violence classification|Academia|int'l|academic|none|0|22K (d)|
|[LifeTox](https://huggingface.co/datasets/mbkim/LifeTox)|Implicit toxicity detection|Academia|int'l|academic|unk|0|-|
## 6. QA and dialogue

|Dataset|Typical Usage|Provider|Docu.|License|Redist|mod-x|Volume|
|:---|:---|:---:|:---:|:---:|:---:|:---:|:---|
|[KorQuAD 1.0, 2.0](https://korquad.github.io/)|QA|Industry|int'l|all|rd|1|70K / 100K questions|
|[KorWikiTQ](https://github.com/LG-NLP/KorWikiTableQuestions)|Table QA|Industry|int'l|all|rd|0|-|
|[HuLiC](https://github.com/smilegate-ai/HuLiC)|Dialog|Industry|dom.|academic|rd|0|115K turns|
|[OPELA](https://github.com/smilegate-ai/OPELA)|Dialog|Industry|int'l|academic|rd|0|600 (d)|
|[CareCall](https://github.com/naver-ai/carecall-corpus)|Dialog|Industry|int'l|academic|rd|0|10K (d)|
|[CLIcK](https://github.com/rladmstn1714/CLIcK)|Cultural QA|Academia|int'l|all|rd|0|2K QA pairs|
|[KoDialogBench](https://github.com/sb-jang/kodialogbench)|Dialogue benchmark|Academia|int'l|all|rd|0|83K examples|
|[KorNAT](https://huggingface.co/datasets/datumo/KorNAT)|Social value QA|Industry|int'l|academic|rd|0|10K questions|
|[K-MMBench](https://huggingface.co/datasets/NCSOFT/K-MMBench)|Vision-language QA|Industry|int'l|academic|rd|1|4.3K questions|
|[K-Viscuit](https://github.com/ddehun/k-viscuit)|VQA|Academia|int'l|academic|unk|0|-|
|[KoSimpleQA](https://huggingface.co/datasets/bzantium/KoSimpleQA)|Factual QA|Academia|int'l|academic|unk|0|1K questions|
|[KoPIQA](https://huggingface.co/datasets/HAERAE-HUB/Ko-PIQA)|Physical commonsense QA|Academia|int'l|academic|unk|0|441 QA pairs|
## 7. Summarization, Translation, and Transliteration

|Dataset|Typical Usage|Provider|Docu.|License|Redist|mod-x|Volume|
|:---|:---|:---:|:---:|:---:|:---:|:---:|:---|
|[Sci-news-sum-kr](https://github.com/theeluwin/sci-news-sum-kr-50)|Summarization|Academia|dom.|academic|rd|0|50 (p)|
|[Korean Parallel Corpora](https://github.com/jungyeul/korean-parallel-corpora)|MT|Academia|int'l|academic|rd|1|100K (p)|
|[Transliteration Dataset](https://github.com/muik/transliteration)|Transliteration|Academia|dom.|all|rd|0|35K (p)|
|[sae4K](https://github.com/warnikchow/sae4k)|Summarization|Academia|int'l|all|rd|0|50K (p)|
|[OPUS-MT ko-en](https://huggingface.co/Helsinki-NLP/opus-mt-ko-en)|MT|Academia|int'l|all|rd|0|Tatoeba Challenge test sets|
|[Naver News Summary](https://huggingface.co/datasets/daekeun-ml/naver-news-summarization-ko)|Summarization|Academia|none|all|rd|0|-|
|[KoreaScience Summary](https://huggingface.co/datasets/nglaura/koreascience-summarization)|Summarization|Academia|int'l|all|rd|0|-|
|[SSL](https://github.com/SSL-Sign-Language/Korean-Disaster-Safety-Information-Sign-Language-Translation-Benchmark-Dataset)|Sign language translation|Academia|int'l|all|unk|0|-|
|[KPC](https://github.com/HandongSF/KoreanUnificationParallelCorpus)|MT|Academia|int'l|academic|rd|1|131K (p)|
|[KNOTICED](https://github.com/sugyeonge/KNOTICED)|MT error detection|Academia|int'l|academic|unk|0|-|
## 8. Korean in multilingual corpora

|Dataset|Typical Usage|Provider|Docu.|License|Redist|mod-x|Volume|
|:---|:---|:---:|:---:|:---:|:---:|:---:|:---|
|[PAWS-X](https://github.com/google-research-datasets/paws/tree/master/pawsx)|Paraphrase detection|Industry|int'l|all|rd|0|5K / 2K / 2K (p)|
|[SIGMORPHON G2P](https://sigmorphon.github.io/sharedtasks/2020/task1/)|G2P conversion|Competition|int'l|all|rd|0|3.6K / 0.45K / 0.45K (p)|
|[TyDi-QA](https://github.com/google-research-datasets/tydiqa)|QA|Industry|int'l|all|rd|0|11K / 1.7K / 1.7K (p)|
|[XPersona](https://github.com/HLTCHKUST/Xpersona)|Dialog|Academia|int'l|all|rd|0|0.3K (d) / 4.7K (s)|
|[XL-Sum](https://github.com/csebuetnlp/xl-sum)|Summarization|Academia|int'l|all|rd|0|-|
|[MultiCoNER](https://registry.opendata.aws/multiconer/)|NER|Competition|int'l|all|rd|0|178K / 2.6K (s)|
|[MINT](https://sites.google.com/umich.edu/semeval-2023-tweet-intimacy/home)|Sentiment analysis|Competition|int'l|unk|unk|0|2K train/test, 0.5K zero-shot|
|[MASSIVE](https://github.com/alexa/massive)|NLU|Industry|int'l|all|rd|0|1M examples|
|[IWSLT 2023](https://iwslt.org/2023/formality)|MT|Competition|int'l|all|rd|0|3K (p)|
## 9. Speech corpora

|Dataset|Typical Usage|Provider|Docu.|License|Redist|mod-x|Volume|
|:---|:---|:---:|:---:|:---:|:---:|:---:|:---|
|[KSS](https://www.kaggle.com/bryanpark/korean-single-speaker-speech-dataset)|ASR, TTS|Academia|int'l|academic|rd|0|12K (u), 1 speaker|
|[Zeroth](https://github.com/goodatlas/zeroth)|ASR|Industry|int'l|all|rd|0|50+ (h)|
|[Pansori-TEDxKR](https://github.com/yc9701/pansori-tedxkr-corpus)|ASR|Academia|int'l|academic|rd|1|3+ (h)|
|[ProSem](https://github.com/warnikchow/prosem)|SLU|Academia|int'l|all|rd|0|7.1K (u), 2 speakers|
|[ClovaCall](https://github.com/clovaai/ClovaCall)|ASR|Industry|int'l|academic|none|0|80+ (h)|
|[JIT/JSS](https://github.com/kakaobrain/jejueo)|ASR, TTS|Industry|int'l|all|rd|0|10K (JSS), 170K (JIT)|
|[kosp2e](https://github.com/warnikchow/kosp2e)|Speech translation|Academia|int'l|academic|rd|0|30K (u)|
|[OLKAVS](https://arxiv.org/abs/2301.06375)|Audio-visual speech recognition|Academia|int'l|all|rd|0|1,150 (h) audio, 5,750 (h) video|
|[KMSAV](https://onlinelibrary.wiley.com/doi/10.4218/etrij.2022-0487)|Audio-visual speech recognition|Academia|int'l|academic|rd|1|150 (h) transcribed, 2,000+ (h) untranscribed|
## 10. Other topics

|Dataset|Typical Usage|Provider|Docu.|License|Redist|mod-x|Volume|
|:---|:---|:---:|:---:|:---:|:---:|:---:|:---|
|[K2NLG](https://github.com/machinereading/K2NLG-Dataset)|Data-to-text generation|Academia|dom.|academic|rd|0|4K (s)|
|[KommonGen](https://github.com/nlpai-lab/KommonGen)|Common sense generation|Academia|int'l|all|rd|0|43K train, 2K test|
|[KoCHET](https://github.com/Gyeongmin47/KoCHET-A-Korean-Cultural-Heritage-corpus-for-Entity-related-Tasks)|Cultural heritage entity tasks|Academia|int'l|academic|unk|0|NER 112K, RE 39K, ET 113K|
|[LBox Open](https://github.com/lbox-kr/lbox-open)|Legal language understanding|Academia|int'l|academic|rd|0|150K precedents|
|[Korean GEC dataset](https://github.com/soyoung97/standard_korean_gec)|GEC|Academia|int'l|academic|rd|0|155K (s pair)|
|[Korean Ambiguity Dataset](https://github.com/bareun-nlp/korean-ambiguity-data)|Word sense disambiguation|Academia|int'l|all|rd|0|35K (s), 8.2K surface forms|
|[KorMedMCQA](https://huggingface.co/datasets/sean0042/KorMedMCQA)|Medical QA|Academia|int'l|academic|rd|1|7.5K questions|
|[KBMC](https://arxiv.org/abs/2403.16158)|Medical NER|Academia|int'l|academic|unk|0|-|
|[ESG-Kor](https://aclanthology.org/2024.findings-emnlp.387/)|ESG information extraction|Academia|int'l|academic|rd|0|119K (s)|
|[KBL](https://github.com/lbox-kr/kbl)|Legal language understanding|Academia|int'l|academic|rd|0|3.3K exam examples, 150K precedents|
|[FunctionChat-Bench](https://github.com/kakao/FunctionChat-Bench)|Function calling benchmark|Industry|int'l|all|rd|0|-|
|[KCL](https://github.com/lbox-kr/kcl)|Legal reasoning|Academia|int'l|academic|rd|1|283 MCQA, 169 essay questions|
|[KorMedLawQA](https://huggingface.co/datasets/snuh/KorMedLawQA)|Medical law QA|Academia|int'l|academic|rd|0|-|

## 기타 주요 데이터

|번호|데이터 종류| 데이터 설명|          
|:---:|:-----------------:|:-----------------:|
|1|[청와대 국민청원](https://www1.president.go.kr/petitions) 사이트의 [만료된 청원](https://www1.president.go.kr/petitions?only=finished) 데이터 모음|[:octocat:](https://github.com/akngs/petitions)|     
|2|[챗봇용 대화 응답 세트](https://github.com/songys/Chatbot_data)|챗봇용 응답 쌍과 긍부정 태깅|
|3|[영화추천시스템을 위한 데이터 세트](https://github.com/lovit/kmrd)|Synthetic dataset for recommender system created with Naver Movie rating system|
|4|[학습용 뉴스 댓글 데이터](https://www.kaggle.com/junbumlee/kcbert-pretraining-corpus-korean-news-comments)|BERT 모델과 학습에 이용한 11.62G 데이터를 모두 공개|   
|5|[AMR](https://github.com/choe-hyonsu-gabrielle/korean-amr-corpus)|[문서요약에 대한 지침](https://github.com/choe-hyonsu-gabrielle/korean-amr-guidelines)과 데이터 세트|
|6|[네이버쇼핑, Steam 플랫폼 리뷰 데이터](https://github.com/bab2min/corpus/tree/master/sentiment)|감성분석(Sentiment Analysis)을 위한 제품 별, 게임 별 별점과 후기를 수집한 데이터셋|



# 국가적 규모에서 구축한 데이터

|번호|데이터 종류| 데이터 설명|
|:---:|:-----------------:|:-----------------:|         
|1| [우리말샘](https://opendict.korean.go.kr/main)| 이 사전에 대한 설명 [:octocat:](https://github.com/songys/Dictionaries) : 다양한 어휘와 유의어 정보 등을 얻을 수 있는 대사전 : 로그인 후 전체 사전 데이터 다운로드 가능|      
|2| [NIA 사전](https://kbig.kr/portal/kbig/knowledge/files/bigdata_report.page?bltnNo=10000000016451)|묻지도 따지지도 않고 다음 링크에서 엑셀로 다운로드 가능 |  
|3| [국립국어원 언어정보나눔터](https://ithub.korean.go.kr/user/total/database/corpusManager.do )| 로그인 후 세종2007 코퍼스나 낭독체 음성 파일 등도 다운로드 가능, 다운 받을 때 간단한 서약에 체크만 하면 되는데 자료의 크기를 작게 나누어 놓아서 여러번 체크해야 한다는 것이 단점 |  
|4| [AIHub](https://www.aihub.or.kr/)| 텍스트와 음성 멀티모달까지 가장 광범위한 데이터, 로그인 및 사용 목적과 기간을 명시한 사용 신청서 작성 후 허가 메일이 오면(하루 정도 걸린다) 다운로드 가능. 개별 데이터 종류와 분량은 자주 갱신되므로 위 사이트에서 최신 목록을 확인한다. |   


   
|번호|데이터 종류| 데이터 설명|            
|:---:|:-----------------:|:-----------------:|         
|5|[국립국어원 모두의 말뭉치](https://kli.korean.go.kr/corpus/main/requestMain.do?lang=ko)| 다양한 분석 말뭉치(형태소 분석과 구문 분석 말뭉치 등), 다양한 도메인의 말뭉치(문어, 신문, 구어, 웹), 자연어 추론을 위한 말뭉치(유사 문장) 등 다양한 데이터들이 체계적으로 구축되어 있다. 말뭉치 종류와 분량은 자주 갱신되므로 위 신청 페이지에서 최신 목록을 확인한다. 로그인, 메일 인증을 거쳐 데이터를 신청할 수 있고 다운로드 받기 위해서는 연구과제명과 수행기관, 약정 기간 등이 필수 입력 요소이다. |

저작권 : 국어원이 승인한 이용 범위 내에서만 저작물을 낼 수 있으며 저작물을 내는 경우 국어원의 정보 제공 사실을 명시 필요, 즉 말뭉치 신청시 명시하면 학습에 사용할 수 있음, 그런 경우에도 아이디등을 제외한 텍스트 자체를 재배포 하는 것은 금지됨, AIHUB의 경우 회원 가입 절차 후에 승인을 받는 절차가 간소화되어 있음.

# 인용 (Citation)

이 자료를 인용할 때는 다음을 사용한다. ACL Anthology 판과 [arXiv 판](https://arxiv.org/abs/2012.15621) 중 하나를 쓰면 된다.

    @inproceedings{cho-etal-2020-open,
        title = "Open {K}orean Corpora: A Practical Report",
        author = "Cho, Won Ik  and
          Moon, Sangwhan  and
          Song, Youngsook",
        booktitle = "Proceedings of Second Workshop for NLP Open Source Software (NLP-OSS)",
        month = nov,
        year = "2020",
        address = "Online",
        publisher = "Association for Computational Linguistics",
        url = "https://www.aclweb.org/anthology/2020.nlposs-1.12",
        pages = "85--93",
    }

    @article{cho2026open,
        title = "Open {K}orean Corpora: A Practical Report",
        author = "Cho, Won Ik and Moon, Sangwhan and Song, Youngsook",
        journal = "arXiv preprint arXiv:2012.15621",
        year = "2026",
        note = "v3, revised 9 Jun. 2026",
        url = "https://arxiv.org/abs/2012.15621",
    }   
