# interpark-macro

![KakaoTalk_Photo_2024-06-11-22-33-03](https://github.com/channnny/interpark-macro/assets/30282985/273fc49e-0619-4610-9cf1-96fe56b790ef)


파이썬으로 구동하며 0~1초 사이 무작위 시간을 간격으로 좌석을 확인하여(새로고침) 원하는 좌석의 등급 및 인원수에 맞는 좌석을 예매할 때까지 반복하는 인터파크 취켓팅 매크로이다.


 ## Parameter
 `main.py` 파일에서 설정할 수 있다.
 | Parameter | DataType | Default | Desc |
| :----- | :---- | :---- | :---------- |
| NEED_SEAT_CNT  | INT  | 2 | 필요한 좌석 수(한자리이면 1, 연석일 경우 2, 세자리일 경우 3 ...) |
| OFFSET  | INT  | 20 | 좌석 클릭 후 버튼이 커지는 현상으로 x 좌표 간격 조정 값(해상도/콘서트장 별로 상이할 수 있음) - 27인치 모니터 기준 |
| ALARM  | BOOLEAN  | TRUE | 취켓팅 성공 후 알람 유무 |


 ---
 
 ## Usage
 1. "좌석 영역 선택 하기" 버튼을 클릭한다.
    + 아래의 방법으로 예약할 좌석의 전체 이미지를 캡쳐한다.
    + 좌상단에 마우스 포인터를 두고 키보드 "a"를 누른다.
    + 우하단에 마우스 포인트를 두고 키보드 "b"를 누른다.
    + 정상적으로 완료된 경우 매크로 프로그램 왼쪽에 캡쳐된 이미지를 확인할 수 있다.
 2. "좌석 등급 선택 하기" 버튼을 클릭한다.
    + 예약할 좌석의 등급(색상)에 마우스 포인트를 올리고 키보드 "a"를 누른다.
    + 예약할 좌석의 등급(색상)이 2개 이상인 경우 위의 방법을 반복한다.
    + 등급(색상)을 모두 지정했다면 "c"를 눌러 등급 선택을 마친다.
    + 정상적으로 완료된 경우 2번 ListBox에 색상 리스트가 업데이트 된 것을 확인할 수 있다.
 3. "좌석 새로고침 좌표 가져오기"를 클릭한다.
    + 인터파크 페이지에서 "좌석 다시 선택" 버튼에 마우스 포인트를 두고 "a"를 누른다.
 4. "좌석 선택 완료 좌표 가져오기"를 클릭한다.
    + 인터파크 페이지에서 "좌석 선택완료" 버튼에 마우스 포인트를 두고 "a"를 누른다.
 5. "매크로 시작" 버튼을 눌러 매크로를 시작한다.
 6. "매크로 중지" 버튼을 눌러 매크로를 종료할 수 있다.
    + ";" 키를 누르면 직접 클릭하지 않고 매크로를 종료할 수 있다.

> ***실전에 적용하기 전에 미리 다른 콘서트나 뮤지컬에 테스트 해보는 게 좋다.***
