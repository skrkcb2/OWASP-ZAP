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
  #### 보고서 출력 예시 (ZAP-Report-.html) .html로 작성되어 나옵니다.
 - ### 검사 결과를 통한 동적 검사 와 정적 검사 비교
   #### 같은 사이트를 두고 ZAP을 통한 동적 검사(DAST) 결과, Fortify on Denamd의 정적 검사(SAST) 결과 입니다.
   ![크기변환 checksdf](https://github.com/user-attachments/assets/39130b5b-1c88-4178-8e52-d0498b978ab2)![크기변환 크기변환 static_Res](https://github.com/user-attachments/assets/8ef7cb38-21d4-4096-951a-c554a1697761)
   #### 위와 같이 Fortify와 같은 정적 분석 도구는 Unreleased Resource 취약점을 효과적으로 탐지할 수 있지만, 동적 분석(DAST)에서는 이를 발견하기 어려울 수 있습니다.
   #### 반면, 정적 분석은 코드의 흐름만을 기반으로 하기 때문에, 함수(API) 호출 시 실제 동작을 정확히 예측하지 못해 File Traversal이나 Remote File Inclusion(RFI) 공격을 놓칠 가능성이 있습니다.
   #### 따라서, 정적 분석(SAST)과 동적 분석(DAST)을 병행하여 보안 검사를 수행하는 것이 가장 효과적인 접근 방식임을 배웠습니다. 앞으로는 탐지 앱의 플러그인과 같은 추가 도구를 활용해 상호 검증을 강화하고, 보안 검사의 완성도를 더욱 높여가는 방식을 생각 하였습니다.




 



  
  

