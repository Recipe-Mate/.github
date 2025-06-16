# 🎓 Recipe-Mate Wiki
본 프로젝트는 On-Device AI 기반의 식재료 관리 및 개인 맞춤형 레시피 추천 앱으로, 사용자의 영수증을 자동 인식하여 식재료를 효율적으로 관리하고 건강 목표에 따른 레시피를 제공하는 서비스를 개발하였습니다.

## 1. 프로젝트 개요
- **프로젝트명:** Recipe-Mate
- **주제:**  OCR 기술을 활용하여 영수증에서 식재료를 자동 추출하고, AI 기반 레시피를 추천하는 스마트 식재료 관리 시스템
- **개발 기간:** 2024.09~2025.06
- **팀원:** 


 <div align="center">
  <table>
    <tr>
      <td align="center" style="padding: 20px;">
        <a href="https://github.com/codingmy" target="_blank">
          <img src="https://avatars.githubusercontent.com/u/97686638?v=4" width="120px" style="border-radius: 50%;" alt="최민영"/><br />
          <h3 style="margin: 10px 0 5px; color: #007acc;">최민영</h3>
        </a>
          <p style="margin: 5px 0; font-size: 14px; color: #888;">PM/BE</p>
      </td>
      <td align="center" style="padding: 20px;">
        <a href="https://github.com/
jaeyoung-leee" target="_blank">
          <img src="https://github.com/user-attachments/assets/91699b42-4f1d-428a-a0c0-e68ae29d70ed" width="120px" style="border-radius: 50%;" alt="이재영"/><br />
          <h3 style="margin: 10px 0 5px; color: #007acc;">이재영</h3>
        </a>
          <p style="margin: 5px 0; font-size: 14px; color: #888;">AI</p>
      </td>
      <td align="center" style="padding: 20px;">
        <a href="https://github.com/Sirius912" target="_blank">
          <img src="https://github.com/user-attachments/assets/a174f883-0f04-4875-b1bd-144d62150a05" width="120px" style="border-radius: 50%;" alt="강지은"/><br />
          <h3 style="margin: 10px 0 5px; color: #007acc;">강지은</h3>
        </a>
          <p style="margin: 5px 0; font-size: 14px; color: #888;">FE</p>
      </td>
      <td align="center" style="padding: 20px;">
        <a href="https://github.com/Korin23574" target="_blank">
          <img src="https://github.com/user-attachments/assets/34d2b446-1a2e-4023-b528-a55c73897e56" width="120px" style="border-radius: 50%;" alt="정시훈"/><br />
          <h3 style="margin: 10px 0 5px; color: #007acc;">정시훈</h3>
        </a>
          <p style="margin: 5px 0; font-size: 14px; color: #888;">FE</p>
      </td>
    </tr>
  </table>
</div>


[**🔗RecipeMate-BE 바로가기**](https://github.com/Recipe-Mate/RecipeMate-SERVER)


[**🔗RecipeMate-FE 바로가기**](https://github.com/Recipe-Mate/RecipeMate-WEB)


[**🔗RecipeMate-AI 바로가기**](https://github.com/Recipe-Mate/RecipeMate-AI)


---

## 2. 작품 개발 동기 및 목적
- **문제 상황 설명:**  
  바쁜 현대인, 특히 1인 가구, 직장인, 학생 등은 식재료를 구매하고도 효율적으로 관리하지 못해 식재료를 버리거나 요리를 포기하는 경우가 많음.
  
- **작품 개발 필요성:**  
  식재료 관리의 불편함을 해소하고, 소비자에게 쉽고 빠른 레시피 추천 서비스를 제공하여 음식물 쓰레기를 줄이고 요리 접근성을 높이고자 함.
  
- **개발 목표 및 기대 효과:**  
  - OCR을 활용한 영수증 자동 식재료 등록
  - 보유 식재료 기반 레시피 추천
  - 사용자 맞춤 식단 제안
  - 식재료 낭비 감소 및 건강한 식습관 유도

---

## 3. 관련 기술 및 선행 연구
- **사용 기술 스택:**
  - Java, Spring Boot, MySQL, AWS S3, JWT 인증, 카카오 소셜 로그인
  - React Native (모바일 클라이언트 및 AI), javaScipt
  - 협업툴 :  Notion, Figma, Github
 
- **유사 서비스 및 차별점:**
  - 만개의 레시피: 키워드 검색 기반 (보유 식재료 반영 불가)
  - 냉장고 관리 앱: 수동 입력 불편, 영수증 자동 등록 부재
  - 스마트 냉장고: IoT 기기 구매 필요, 접근성 제한


- **시장 동향 및 수요 근거:**
  - 1인 가구 증가: 2023년 기준 전체 가구의 35.5%  
  - 건강식 수요 증가: 2023년 건강기능식품 시장 5조 4,240억 원, 연평균 5.8% 성장  
  - 출처: [통계청](https://kostat.go.kr), [식품산업통계정보](https://www.aTFIS.or.kr)


---

## 4. 시스템 설계 및 개발
- 시스템 아키텍처
  
![Image](https://github.com/user-attachments/assets/3a0edc70-319f-42ba-b31e-45aba937c9d4)

- ERD (데이터베이스 설계)
  
![Image](https://github.com/user-attachments/assets/d03961dd-c929-4d28-93f5-efcc8c055bdc)

- UI/UX 와이어 프레임
   
![Image](https://github.com/user-attachments/assets/d14de9ed-14bd-41bb-828d-a44e1e1d5f51)

---

## 5. 구현 결과

#### ✅ 카카오 소셜 로그인
- 카카오 소셜 로그인을 연동하여 간편한 회원가입 및 로그인 기능을 제공합니다.
- OAuth 2.0 기반 인증 방식을 적용하여 보안성과 사용자 편의성을 확보하였습니다.

#### ✅ 영수증 기반 식재료 자동 등록
- `react-native-image-picker`를 활용하여 사용자가 영수증 이미지를 직접 촬영 또는 선택할 수 있습니다.
- `react-native-ml-kit/text-recognition`을 활용하여 On-Device OCR로 영수증 내 텍스트를 빠르고 안정적으로 추출합니다.
- 정규표현식 및 후처리 로직을 통해 브랜드명, 제품명, 수량, 용량 정보를 자동으로 분리·정제하여 식재료 데이터로 등록합니다.

#### ✅ 식재료 통합 관리
- 실온, 냉장 보관 식재료를 모두 관리할 수 있도록 설계하여, 사용자의 보유 식재료를 직관적으로 확인할 수 있습니다.
- 식재료의 보관 현황, 소비 일정, 등록·삭제 기능을 제공하여 효율적인 재고 관리가 가능합니다.

#### ✅ 개인 맞춤형 레시피 추천
- 사용자가 설정한 건강 목표 (예: 체중 관리, 단백질 섭취 강화 등)를 기반으로 보유 식재료를 활용한 레시피를 추천합니다.
- 부족한 재료가 있을 경우, 생성형 AI를 활용하여 대체 가능한 식재료를 제안하여 사용자 선택의 폭을 넓힙니다.

#### ✅ 사용자 데이터 기반 관리
- 사용자의 식재료 보유 현황, 레시피 사용 이력, 식재료 소비 패턴 등의 데이터를 관리하여, 향후 맞춤형 서비스 고도화를 위한 기반을 구축합니다.

---
