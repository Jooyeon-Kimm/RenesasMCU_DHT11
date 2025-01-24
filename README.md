# RenesasMCU_DHT11
Receives temperature and humidity data every minute and activates the LED and buzzer when certain conditions are met.  
1. MCU를 사용해 온도 및 습도를 측정하고, 측정 데이터를 실시간으로 UART로 출력  
2. 일정 기준 이상의 온도나 습도 변화가 발생할 경우 경고 LED와 부저를 통해 알림 제공  

1. 센서 연동  
  - DHT11(온도 및 습도 센서)에서 데이터 수신을 위한 디지털 인터페이스 구현  
2. 실시간 데이터 처리  
  - 온도 및 습도 데이터를 1초 간격으로 측정하여 UART로 PC에 실시간 업데이트  
  - 과거 1분 동안의 데이터를 MCU 내부 메모리에 저장하고 이를 평균 내어 표시  
3. 알림 기능  
  - 온도가 30도 이상일 때 LED를 깜빡이기  
  - 습도가 80% 이상일 때 부저 울리기  

환경: e2studio  
언어: C  
실행파일: DHT11_Demo.zip  
UI: LVGL  

시연 영상:
https://youtube.com/shorts/0kAwfqPc5go?feature=share
