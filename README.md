# 자동차 경주 게임
    프로그램 시작 시 n개의 자동차 이름과 횟수를 입력받는다
    자동차들은 매 회마다 랜덤으로 전진, 정지를 결정한다
    사용자가 정한 count만큼 게임이 진행되면 가장 많이 진행한 자동차가 승리한다


## 프로그램 흐름
    1. 유저로부터 입력받은 문자열을 슬라이싱하여 자동차 이름 분리
    2. 시도할 횟수를 입력받아 게임 시도 횟수 제어
    3. n회 게임 시도 후 각 인스턴스 객체의 위치를 비교하여 우승 자동차 선정

## 만들 메소드
- 문자열을 입력받아 슬라이싱하여 문자열 배열로 리턴하는 메소드
        
        경주할 자동차의 갯수를 입력받지 않고 슬라이싱하며 추가해야하기 때문에
        배열보다는 리스트의 사용이 적합
        -----------------------------------------------------------------
        String 클래스의 Split method가 배열초기화의 iteration을 수행하므로
        String 배열을 사용해도 무방
              
- 0~9사이의 유사난수를 구하고 자동차의 전진 여부를 결정하는 메소드

        Car클래스의 메소드로 구현할지 다른 클래스로 분리할지 미정
        ------------------------------------------------------------------
        테스트 및 메인함수에서 반복문을 줄이기 위하여 Car클래스의 메소드가 아닌
        UtiliyMethods 클래스로 분리
        
- 게임 수행회수를 가르키는 Int 변수를 매개변수로 받아 게임 반복 수행을 제어하는 메소드
        
        메인 메소드를 가볍게 하기 위한 기능 분리
        
- 리스트에 존재하는 Car객체들의 position을 비교하여 우승 자동차를 선정하는 메소드

        클래스 분리와 Static 메소드를 이해하기 위해 Static하게 구현

        
