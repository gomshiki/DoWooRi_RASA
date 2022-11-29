# RASA 오픈 소스를 이용한 업무 비서 챗봇

챗봇을 이용해 기안문(연차, 반차, 사직, 휴직)을 작성하고, 웹페이지에서 결재할 수 있는 서비스 입니다.


## 개발 환경 및 사용 라이브러리

- OS : windows10
- Anaconda 가상환경
- Rasa 2.8.27
- Mecab-konlpy

## 사용방법

### Anaconda 가상환경 설정
   - anaconda 다운로드
   - anaconda prompt 실행
   - anaconda 가상환경 설정 -> conda create –n 가상환경이름 python==3.7.9   
   - 각종 라이브러리 설치 
	    	
	pip install -U pip setuptools wheel (pip 업데이트)
    	pip install rasa==2.8.27 (RASA 설치)
    	
	pip install spacy (spacy 모델 설치)
    	
	pip install https://github.com/explosion/spacy-models/releases/download/xx_sent_ud_sm-3.2.0/xx_sent_ud_sm-3.2.0-py3-none-any.whl (space 모델 설치)
	
	pip install https://github.com/explosion/spacy-models/releases/download/xx_sent_ud_sm-3.2.0/xx_sent_ud_sm-3.2.0.tar.gz (space 모델 설치)
	
	conda install –c conda-forge spacy-model-ko_core_news_sm (한국어 spacy 모델 설치)
    	
	pip install konlpy (형태소 분석기 라이브러리 설치)
    	
	형태소분석기(mecab) 설치
	설치 링크 : https://hong-yp-ml-records.tistory.com/91
	    
## custom_tokenizer.py 옮기기
    - 경로 : C:\Users\[사용자]\anaconda3\envs\[가상환경]\Lib\site-packages\rasa\nlu\tokenizers
    
## Anaconda prompt로 Rasa 실행하기
    - prompt 창 두개 실행 후 RASA가 설치된 가상환경 실행
    - prompt 각 창에 아래 명령어 실행
    	rasa run actions
	rasa run -m model --enable-api --cors "*" -vv
