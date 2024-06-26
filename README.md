# <OpenSource_Team16><br/>
24-1 오픈소스프로그래밍 기말 팀 프로젝트 <br/>
YOLO POSE 기반 독거노인 쓰러짐 발견 및 알림 소프트웨어
<br/><br/>

### OpenSource_16.py
> 최종본<br/>
> test_05(sample).py와 동일한 파일

*이하 테스트 파일은 test폴더에 있음.</br>
<br/>

# 실행방법

1. 저장소를 복제하거나 스크립트를 다운로드하세요. (OpenSource_16.py)
2. 필요한 실행 환경을 구축합니다. (하단에 서술)
3. 사전 학습된 YOLOv8 모델(.pt)이 있는지 확인하고 스크립트에 해당 경로를 제공하세요.
4. 다음 명령을 사용하여 스크립트를 실행합니다: python OpenSource_16.py
5. 웹캠이 활성화되고 물체 감지 오버레이가 포함된 라이브 비디오가 표시됩니다.
6. 프로그램을 종료하려면 'ESC' 또는 'q'를 누르세요.
<br/>


# 실행환경 구축
스크립트를 실행하기 전에 다음 환경이 준비되어 있는지 확인하세요.

- 파이썬
- 오픈CV (pip install opencv-python)
- 울트라리틱스 (pip install ultralytics)
- pip install lap(lapx)

<br/>

### <<파일 실행 전 yolov8s-pose.pt 설치>> 
- 사전 학습된 YOLOv8 모델
- 스크립트(OpenSource_16.py)에 파일 경로 제공

<br/>

### <<이메일 정보 입력>> (OpenSource_16.py 파일 내 수정 필요)

- mail_user = '경고 메시지 보낼 이메일 계정'<br/>
- email_password = '보낼 계정의 비밀번호'<br/>
- recipient_email = '경고 메시지 받을 이메일 계정'
  <br/>
- 경고 메시지 보낼 계정 관리 > 보안 > 보안 수준이 낮은 앱의 액세스 허용<br/>
- (gmail 뿐 아니라 다른 이메일 계정도 가능)

<br/><br/>
================================================================

## 이하 테스트파일 설명

### test_05(sample).py
> test_03.py 배경으로 제작
> 파일 내 수정 필요
> > email_user = '경고 메시지 보낼 이메일 계정'<br/>
> > email_password = '보낼 계정의 비밀번호'<br/>
> > recipient_email = '경고 메시지 받을 이메일 계정'<br/>

> 경고 메시지 보낼 계정 관리 > 보안 > 보안 수준이 낮은 앱의 액세스 허용

### test_03.py
> interface는 app.py이고 기능은 test_02.py의 fall detection으로 가져와 합침<br/>
> classes.txt 설치 필요 없음<br/>

### test_02.py
> https://www.youtube.com/watch?v=wrhfMF4uqj8<br/>
> 위 영상 기반으로 제작

> 웹캠으로 인식하도록 수정함<br/>
> pip install cvzone 해야함<br/>
> classes.txt 설치 필수<br/>

### On Video.py
> 실행하려면 경로 재설정 해야함<br/>
> 비디오에 프레임을 씌워서 새로 비디오를 생성<br/>

### open16.py
> 어깨와 엉덩이 좌표값으로 넘어짐을 구분하는 프로그램.</br>
> 웹캠으로 시연하기 어려워서 반려.

### app.py
> 객체 감지 후 사람인지 아닌지를 판별
> 최종 인터페이스로 채택



