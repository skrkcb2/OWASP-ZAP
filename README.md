# OWASP-ZAP
## OWASP-ZAP 이란?
#### OWASP-ZAP은 OWASP에서 제공하는 오픈 소스 보안 테스트 도구입니다. 주로 웹 애플리케이션의 보안 취약점을 발견하고 분석하는 데 사용되며, 보안 전문가나 개발자가 웹 애플리케이션을 자동화된 방식으로 스캔하고 수동 검토를 보완하는 데 사용합니다. 

- ### OWASP-ZAP 을 활용한 동적 검사(DAST)
  #### OWASP-ZAP 흐름
  Zap 은 Spider, Ajax Spider을 통해 사이트 를 크롤링한 후 발견된 모든 URL과 자원을 Acticve Scan, Passive Scan을 통해 분석합니다.
  #### Automated Scan (자동 스캔)
  #### 웹 취약점 확인을 위한 사이트 탐지 진행
  ![AutomateScan](https://github.com/user-attachments/assets/4f18c675-bf21-4faa-ab8c-42207c25185a)
  #### 탐지 간략 예시
  ![20250214_152525](https://github.com/user-attachments/assets/99bd5a0a-5748-4b55-bc9f-edd09443c1ca)
  #### 탐지 결과 
  ![AutomateRes](https://github.com/user-attachments/assets/e21e60fd-12a7-408c-9dde-29d3fd019255)  
  해당 스캔을 통해 대략적인 취약점은 확인되었지만, 유도된 취약점은 아직 발견되지 않았습니다. 따라서 Active Scan을 통해 추가 검수를 진행
  #### Active Scan (특정 타켓 심층 검사)
  ![20250214_153612](https://github.com/user-attachments/assets/51264f24-df93-4ede-bb08-d4d75baf3a77)
  #### 보고서 출력 예시 (ZAP-Report-.html, ZAP-Report-.pdf(변환하여 CSS 적용 X))

 



  
  

