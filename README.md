프로젝트명
- IoT를 이용한 차량정보 전송 및 활용

상세 내용
- ESP32와 CAN Tranceiver를 통해 차량 CAN 통신에 접속하여
  차속, RPM, 냉각수 온도, 총 주행거리, 1번 실린더 상태 등과 같은
  차량의 정보를 웹서버상에 실시간으로 표시한다.
- DB에 저장된 차량 정보를 python 코드를 이용해 
  하루 평균 주행거리, 하루 평균 차속, 하루에 발생하는 급감속, 급가속 같은 정보를 도출한다.
- 이를 통해, 운전자의 운전 습관에 점수를 도출하고 운전자로 하여금 운전 습관을 고칠 수 있도록 도와주는 서비스를 만들어보도록 한다.

현재 진행 상황
- CAN 통신을 사용해 차량에서 각종 정보 추출 성공
- MQTT를 이용해 외부 DB서버에 추출정보 저장 성공
- JavaScript를 사용해 차량 관련 정보를 실시간으로 표시하고 통계정보를 그래프로 표시
- ajax를 이용해 데이터를 참조하는 부분만 갱신 성공
- PHP와 Python으로 DB 데이터를 가공하고 다시 저장

앞으로 할 일
- 차량에서 다 유의미한 차량 데이터 추출
- 추출한 데이터로 유의미한 결론 도출
- 이를 웹페이지에서 시각적으로 표현
