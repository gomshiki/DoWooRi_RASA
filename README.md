# RASA 오픈 소스를 이용한 업무 비서 챗봇

챗봇을 이용해 기안문(연차, 반차, 사직, 휴직)을 작성하고, 웹페이지에서 결재할 수 있는 서비스 입니다.


## 개발 환경 및 사용 라이브러리

- OS : windows10
- Anaconda 가상환경
- Rasa 2.8.27
- Mecab-konlpy

## 사용방법


Anaconda 가상환경 설정
   - anaconda 다운로드
   - anaconda prompt 실행
   - anaconda 가상환경 설정 -> conda create –n 가상환경이름 python==3.7.9   
   - 각종 라이브러리 설치 
	    	
	pip install -U pip setuptools wheel
    	4-3)  RASA 다운로드
    		pip install rasa==2.8.27 
    	4-4) 자연어 처리 라이브러리(SpaCy)
		pip install spacy
    	4-5) spacy 모델 다운로드
	    pip install https://github.com/explosion/spacy-models/releases/download/xx_sent_ud_sm-3.2.0/xx_sent_ud_sm-3.2.0-py3-none-any.whl
	    pip install https://github.com/explosion/spacy-models/releases/download/xx_sent_ud_sm-3.2.0/xx_sent_ud_sm-3.2.0.tar.gz
	4-6) 한국어 spacy model 다운로드
	    conda install –c conda-forge spacy-model-ko_core_news_sm
    	4-7) 한국어 처리를 위한 파이썬 패키지
	    pip install konlpy
    	4-8) 형태소분석기(NLU 전처리 과정) 설치(하기 링크 참고)
	   설치 링크 : https://hong-yp-ml-records.tistory.com/91
	    
