# Korean NLP Tutorial
자연어처리를 공부하며 여러 한국어 NLP Task에 대한 예시 코드를 작성하고자 만들었습니다.  
예시 코드를 통해 자연어처리 분야의 입문자들에게 도움이 되었으면 합니다 :)

## 작업환경
### Library Version
Python == 3.8.5  
Tensorflow == 2.5.0  
KoNLPy == 0.6.0  
### PC environment
OS : WINDOWS 10  
GPU : RTX 3070  
CPU : AMD Ryzen 5 5600X 6-Core Processor 3.70 GHz  

## KoNLPy
한국어 형태소 분석기인 KoNLPy를 사용할 때, 아래와 같은 코드를 입력 시 오류가 발생할 수 있습니다.  
처음 자연어처리를 시작하는 분들은 다음과 같이 KoNLPy를 사용하기 위한 준비과정이 필요합니다.  
```python
from konlpy.tag import Okt
tokenizer = Okt()
```
```python
from konlpy.tag import Komoran
tokenizer = Komoran()
```
---> Error  

1. Install JVM (Java), JDK (Java Development Kit)
2. Set Environment variable Path (JAVA_HOME path)
3. Install JPype -> [[Download Link]](https://www.lfd.uci.edu/~gohlke/pythonlibs/#jpype)  
: 버전에 맞는 JPype를 설치합니다.
4. Install KoNLPy
```python
pip install konlpy
```

## NLP Tasks
- Sentiment Analysis (감성 분석)
- Text Summarization (텍스트 요약)

### Sentiment Analysis
1. Naver Movie Review - LSTM
2. Naver Movie Review - CNN

### Text Summarization
1. (미완성) Book Summarization - Seq2Seq + Attention

## Dataset
- Naver sentiment movie corpus(네이버 영화 리뷰 데이터셋) -> [GitHub e0t/nsmc](https://github.com/e9t/nsmc)
- AI Hub 도서자료요약 데이터셋 -> [AI Hub 도서자료요약 소개](https://aihub.or.kr/aidata/30713)
- 도서자료요약 데이터 csv로 정리 -> [작성자 구글 드라이브 공유 링크](https://drive.google.com/drive/folders/1xKEErru12VNZBH-LK59rsHtke5tWxgQV?usp=sharing)
