# opensw23-강김삼

# Team Introduction
  강윤원 202211249 리더
  
  김소희 202210728 코더
  
  김종혁 202211282 서포터
  
  김민형 202211270 서포터
# Topic Introduction
  - 원본 프로젝트 레포지토리 주소 : https://github.com/smahesh29/Gender-and-Age-Detection.git

  - 주제 : 이미지 및 웹캠 영상으로 부터 성별 및 연령 감지

  - 내용 :
  
    - 딥러닝을 이용한 얼굴 인식 및 이를 이용한 성별, 나이 추정 프로그램이다.
  
    - Tal Hassner과 Gil Levi가 pretrained한 모델을 사용해 성별, 나이를 추정한다.
  
    - 입력받은 이미지 혹은 웹캠의 데이터에서 사람의 얼굴을 감지해 성별, 나이를 추정한다.
  
    - 성별은 male 혹은 female 둘 중 하나로 판단한다.
  
    - 연령은 (0 – 2), (4 – 6), (8 – 12), (15 – 20), (25 – 32), (38 – 43), (48 – 53), (60 – 100) 8개의 구간 중 하나로 판단한다.
    - python detect.py --image <파일명> 의 <파일명>에 jpg 파일 입력 시 일정 시간 후에 output result가 자동으로 팝업됨(output result는 Result 항목의 그것과 동일하게 나옴.)
    - python detect.py로 실행시 일정 시간 후 웹캠이 구동되어 카메라 현황이 팝업됨. 카메라 현황에 실시간으로 성별과 나이가 출력되고 콘솔창에 반영 내용이 실시간으로 출력됨
# Results
  |input data|input|ouput|
  |:---|:---:|:---:|
  |sample data|<img width="362" alt="sample1" src="https://github.com/KangYunWon/opensw23-KangKimSam/assets/127182199/f9516e0e-e243-4891-a9e8-10e6ead64501">|<img width="362" alt="sample1" src="https://github.com/KangYunWon/opensw23-KangKimSam/assets/127183027/58feb0e0-b17d-44fe-9e7a-484f48e9e581">|
  |male(20)|<img width="312" alt="jonghyuck1" src="https://github.com/KangYunWon/opensw23-KangKimSam/assets/127182199/d66de645-1bea-4fb9-9acf-671a72971934">|<img width="312" alt="jonghyuck1" src="https://github.com/KangYunWon/opensw23-KangKimSam/assets/127183027/a451eda9-9313-4f7e-a148-48d22b5ec638">|
  |female(22)|webcam|<img width="312" alt="webcam1" src="https://github.com/KangYunWon/opensw23-KangKimSam/assets/127182199/178094ee-74bb-4dea-b14c-e8cf86604fd8">|


# Analysis/Visualization

# Installation
- 모든 구동은 cmd창에서 진행한다.

- 구동 환경
  - os : window 10, window 11
  - 파이썬 3.9.13
  - lg gram 2021 ver.
  - cpu: 11th Gen Intel(R) Core(TM) i7-1165G7
  - RAM: 16.00GB
  - GPU: intel IRIS xe
 
- 추가 라이브러리 요구사항
  - opencv
  
    `pip install opencv-python`
  - argparse
  
    `pip install argparse`
    
- 구동 방법    
 
  1. repository 복사(cmd의 default path에서 실행함) 

      `git clone https://github.com/KangYunWon/opensw23-KangKimSam.git`
    
  2. repository를 복사하면 cmd의 default path 밑에 opensw23-KangKimSam 디렉터리가 생성됨.
  
  3. 생성된 opensw23-KangKimSam 디렉터리로 이동 후 detect.py파일 실행
  
      - 사진 파일을 이용해 성별, 나이 분석 시

        `python detect.py --image <image_name>`
      
        example
      
          `python detect.py --image girl1.jpg`
          
      - 웹캠을 이용해 성별, 나이 분석 시

        `python detect.py`
    
# Presentation
