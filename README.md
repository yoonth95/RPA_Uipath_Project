# RPA_Uipath_Project
Uipath Hackathon Project

# Contents

## 1. 구직자를 위한 채용정보 이메일 발송 RPA
https://github.com/yoonth95/RPA_Uipath_Project/1.-구직자를-위한-채용정보-이메일-발송-RPA/
#### 1.1 개요
- 웹사이트별로 게시되는 채용 정보의 수가 광범위하고 게시된 형식이 저마다 달라 정보 습득이 어려움
- 구직자에게 필요한 채용 정보를 수집하여 메일로 받아보게 함으로써 정보 검색의 시간을 단축시키고자 함

#### 1.2 순서
- 채용사이트 (사람인, 워크넷, 잡코리아) 접속
- 키워드 입력 후 검색
- Data(기업명, 공고명, 경력유무, 학력, 위치, 기한 등) 수집
- Excel 데이터 필터링 후 다른 이름으로 저장
- 이메일 발송

#### 1.3 발생 문제점
- 각 사이트마다 Selector 편집 사용의 어려움
- 가져올 Data 말고 다른 Data 수집의 어려움 (사이트마다 보여지는 Data가 다르기 때문)
- 엑셀 병합 후 가공하는 과정에서의 실행 시간이 오래걸림 (엑셀을 실행 시키고 일일히 작업해야하기 때문에 시간이 오래걸림)

#### 1.4 업무 흐름도
![image](https://user-images.githubusercontent.com/78673090/133557895-3f7c2694-10f0-47f1-8306-161e032b868e.png)

&nbsp;
## 2. 상품기획 제안서 작성 및 이메일 발송 RPA
https://github.com/yoonth95/RPA_Uipath_Project/2.-상품기획-제안서-작성-및-이메일-발송-RPA/
#### 2.1 개요
- 상품기획자가 타 유통채널에 제품을 영업하고자 할 때, 각 유통채널의 개별 특성 (수수료율, 인기상품 카테고리 등)을 고려하여 상품을 구성한 기획서를 Word로 작성하고 자동으로 이메일 발송
- 다양한 유통채널에 대해 보다 빠르게 접촉하여 일을 진행하도록 도움

#### 2.2 순서
- 거래하고자 하는 업체에서 명함이 첨부된 이메일을 수신하면, 명함 정보 OCR을 이용하여 추출 데이터를 Excel 저장
- 업체명, 수수료율이 들어간 Excel에서 일치하는 업체와 수수료율을 가져와 판매가가 적힌 새로운 Excel 파일을 생성
- 새로 생성된 Excel을 형식화된 Word 문서에 데이터를 삽입하여 상품 기획서를 생성
- 생성된 상품 기획서를 상품 기획자의 명함에서 추출한 이메일로 발송

#### 2.3 발생 문제점
- 2~3일의 짧은 기간 동안 샘플 명함을 제작하고 OCR로 데이터 추출 과정에 대한 프로젝트 시간이 부족하여 정확성이 떨어짐
- 명함 파일의 경우 플랫폼마다 명함 종류가 다르기 때문에 RPA로 통일화 시킨다는 것에 대한 어려움
- 머신러닝을 진행하여 OCR의 정확도를 높여야 함

#### 2.4 업무 흐름도
![image](https://user-images.githubusercontent.com/78673090/133558869-cf33743d-a5d3-4a2c-bee9-1f362e73f87e.png)
