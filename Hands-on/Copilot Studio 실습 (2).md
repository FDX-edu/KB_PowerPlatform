# 3. Copilot Studio 실습

## 1) Copilot Studio에 로그인

```
https://aka.ms/CopilotStudioStart
```
또는
```
https://copilotstudio.microsoft.com
```
해당 URL로 이동하여 로그인 합니다.

## 2) 에이전트 생성

1. Microsoft Copilot Studio 홈에서 **만들기** - **새 에이전트**를 클릭합니다.

   <img src="https://github.com/user-attachments/assets/4be673c9-cb7e-467e-99c6-eb4d57d5913d" width=500/>

3. 만약 아래 이미지와 같은 대화형 생성 환경이 나타난다면 **구성으로 건너뛰기**를 클릭합니다. </br>
   (나타나지 않으면 이 단계는 무시합니다.)

   <img src="https://github.com/user-attachments/assets/1a963669-0734-4b51-abcc-5a52b8056431" width=800/>
   
5. 에이전트의 **이름**을 입력하고, **만들기**를 클릭합니다.

    <img src="https://github.com/user-attachments/assets/2bb04b0e-713e-4399-bb2d-8c2bbe616521" width=800/>

    에이전트 이름은 **[아이디] Agent(classic)** 으로 지정합니다. </br>
    언어 설정은 한국어에서 변경하지 않습니다.</br>
    설정이 마무리되었으면 **만들기**를 클릭합니다.
   ```
   [아이디] Agent(classic)
   ```

6. 에이전트가 만들어졌습니다.</br></br>



## 3) 지식 소스 업로드 및 활용
### ① Files

1. [qna.xlsx]()를 다운로드합니다.</br>

2. 에이전트의 **참조 자료**(Knowledge) 탭으로 이동하여 **참조 자료 추가**(Add knowledge)를 선택합니다.

    <img src="https://github.com/user-attachments/assets/783f85cc-2895-4453-9001-df185a32ccaa" width=800/>

3. **파일 업로드** 부분에 qna.xlsx 문서를 업로드한 다음 **추가**를 클릭합니다.

   <img src="https://github.com/user-attachments/assets/8e743708-51c2-4bef-8ee2-3129437a203a" width=800/>
    
    **상태**가 **준비**로 될때까지 시간이 필요합니다.</br>
    (기다리는 시간 동안 [다른 작업](#3-SharePoint)을 수행해도 됩니다)

    <img src="https://github.com/user-attachments/assets/839bafc0-28cc-4285-b60c-e65addb5f98b" width=800/>

    💡참고</br>
    상태가 **알 수 없음**으로 나타나는 경우도 있습니다. 이 경우에도 정상적으로 파일이 업로드되는 중이니 기다리면 됩니다.

1. 상태가 **준비**가 되었다면, 에이전트를 테스트해봅시다.</br>
   아래와 같은 질문을 합니다.
   
   ```
   철산군의 역사는 어떻게 되나요?
   ```
   ```
   문화재를 보존하기 위해 시행하는 법은 무엇인가요?
   ```

4. 참조의 데이터 소스를 눌러 각 질문에 맞는 지식 소스와 위치를 참조했음을 확인할 수 있습니다.

    <img src="https://github.com/user-attachments/assets/48b9b0c7-9d4a-4887-8ead-a345372fe05f" width=800/>

### ② 웹사이트

1. **참조 자료**(Knowledge) 탭으로 이동합니다.
   
    **+ 참조 자료 추가**를 클릭한 후 **공개 웹 사이트** 를 클릭하여, 다음 웹사이트를 추가하세요.
    ```
    https://learn.microsoft.com/ko-kr/microsoft-copilot-studio/
    ```
    <img src="https://github.com/user-attachments/assets/108ee567-0f1d-40ec-8669-5144f27e1335" width=800/>

1. 파일 업로드와 다르게 곧바로 **준비** 상태가 됩니다. 에이전트를 테스트해 봅시다.

   아래와 같은 질문을 연달아서 해 보세요.

   ```
   코파일럿 스튜디오란?
   ```
   ```
   지원하는 언어는 무엇인가요?
   ```
   
3. 답변을 생성하고 답변의 근거가 되는 참조를 포함하며, 사용자에게 답변을 생성하는 데 사용된 소스의 링크로 이동할 수 있는 옵션을 제공합니다.

   <img src="https://github.com/user-attachments/assets/0220d5ae-87e1-49d6-bfc4-b120d9054cac" width=600/>

   또한, 에이전트가 두 번째 답변을 생성할 때, 첫 번째 질문과 답변의 문맥을 이해하고 생성하였음을 확인할 수 있습니다.

   ※ 참고: 에이전트가 링크를 참조하지 않고 일반 지식으로만 답변을 수행한 경우, 참조 자료가 완벽한 준비 상태가 아닐 수 있습니다.</br>
   일 분 정도 기다렸다가 재시도해주세요


### ③ SharePoint

1. **참조 자료(Knowledge)** 탭으로 이동하여 **참조 자료 추가(Add knowledge)** 를 클릭합니다.</br>
   **공무원 휴가제도.pdf** 을 추가합니다.

   <img src="https://github.com/user-attachments/assets/0e0c56c1-42d6-4e70-9a34-8bb2df52cae8" width=800/>


1. **준비** 상태가 된 후 에이전트를 테스트해 봅시다.

   아래와 같은 질문을 해 보세요.

   ```
   공무원 휴가의 휴가일수에 대해 알려주세요.
   ```
   ```
   특별휴가의 종류를 알려주세요.
   ```
   
   <img src="https://github.com/user-attachments/assets/5973d9a1-8949-447c-ba9d-411db3d70977" width=600/>

   ※ 참고: 기존의 상용화된 pdf 파서 등에서 제대로된 결과를 내지 못하는 병합된 셀의 데이터도 제대로 이해하고 결과를 출력함을 확인할 수 있습니다.
   
   ```
   경조사 휴가의 일수를 알려주세요.
   ```
   
   <img src="https://github.com/user-attachments/assets/1e1e88b3-e3a8-4239-be46-ea9ca1aba495" width=800/>
