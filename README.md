# Posture-Correction-Device

목 뒤에 부착하여 몸이 좌우로 기울어지거나(MPU-6050으로 검출), 목이 휜 경우(거북목 현상, 휨 센서를 이용하여 검출) 사용자에게 진동 PWM 제어를 통해 알림을 주어 자세를 교정할 수 있도록 하는 장치입니다.
일정 시간 이상(3초) 지속될 경우 알림이 가도록 하였는데, 모든 정보는 SD 카드의 메모리 영역에 저장되도록 직접 write하였습니다.

ATmege4809를 사용하여 설계하였습니다.

main코드의 setup 함수 내에 getLogs(); 의 주석을 해제하면 main 코드만으로 sd카드 열람과 "자세 교정 도움 장치"를 모두 구현할 수 있습니다.
