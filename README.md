# Google-Cloud
How to use Google Cloud Service

<hr>
<details>
  <summary>Google Compute Engine</summary>
  <br>
  <b>클라우드 서버 만들기</b>
  <b>머신 구성</b>
  <ol>
    <li>인스턴스 생성</li>
    <li>지역 선택 - 서울</li>
    <li>머신 선택 - E2(저렴함)</li>
    <li>머신 유형 선택 - E2-small(테스트용)</li>
    <li>인스턴스 생성하기</li>
  </ol>
  <b>네트워킹</b>
  <ol>
    <li>HTTP 트래픽 허용</li>
    <li>HTTPS 트래픽 허용</li>
  </ol>

  mqtt 브로커 사용시
  VPC 네트워크 - 방화벽 -방화벽 규칙 만들기 - 이름설정 - 네트워크 디폴드 - 우선순위 1000 - 대상? - 소스 ip 범위 외부에서 접속 허용하려면 0.0.0.0/0 - 프로토콜 및 포트 tcp:1883
sudo apt-get install mosquitto mosquitto-clients -y

sudo systemctl status mosquitto
sudo nano /etc/mosquitto/mosquitto.conf

listener 1883
allow_anonymous true 
두줄 추가

sudo systemctl restart mosquitto
재시작


  
   <ol>네트워크
    <li>인스턴스 생성</li>
    <li>지역 선택 - 서울</li>
    <li>머신 선택 - E2(저렴함)</li>
    <li>머신 유형 선택 - E2-small(테스트용)</li>
    <li>인스턴스 생성하기</li>
  </ol>
  <br>
  <b>쉘에서 업데이트 및 자바 설치 후 버전 확인</b>
  <ol>
    <li>sudo apt-get update</li>
    <li>sudo apt-get install openjdk-17-jdk -y</li>
    <li>java -version</li>
    <li>Spring Boot 프로젝트 빌드 후 jar 파일 업로드</li>
    <li>sudo nohup java -jar 파일이름.jar & <b>백그라운드로 서버 구동</b></li>
  </ol>
  
</details>

<details>
  <summary>Google Cloud SQL</summary>
  <br>

  엔터프라이즈 - 샌드박스 - 아이디, 비번 설정 - vCpu1개 , 3.75gb 제일싼거 - 용량 10gb 싼거 ssd - 연결 네트워크 이름 설정 및 sql 이랑 연결할 서버가 있는 외부 ip/32 입력 (32는 하나만 허용한다는 의미) - 생성

  
</details>

<details>
  <summary>Google Cloud Storage</summary>
  <br>
</details>
