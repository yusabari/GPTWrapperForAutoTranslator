# GPTWrapperForAutoTranslator
ChatGPT 번역을 웹 API 형태로 쓰기 위해 만들어진 Python 스크립트입니다.

[AutoTranslator](https://github.com/bbepis/XUnity.AutoTranslator)등의 사용자 정의 Endpoint 지정 가능한 번역 플러그인에 사용할 용도로 만들어졌습니다.
# 필수 환경
* 이지트랜스 (최소 한번 실행 필수)
* Python
* Flask

# 주의
* 해당 스크립트를 절대 외부망으로 노출하거나 서비스 하지 마시기 마랍니다. 보안 문제가 있을 수 있습니다.

# 사용 방법
실행 전 trans.py 파일을 수정하여 API_KEY 및 TRANSLATION_PROMPT 를 수정해주세요.
필수 환경이 다 갖춰진 상태라면, 명령 프롬프트에서 `python trans.py`로 실행할 수 있습니다.

기본값은 127.0.0.1을 호스트로, 5000번 포트에서 동작합니다.
# XUnity.AutoTranslator와 사용
다음과 같은 커스텀 엔드포인트를 추가해주세요.
```
Endpoint=CustomTranslate
[Custom]
Url=http://127.0.0.1:5000/translate
```
# Special Thanks to
* [ezTransWeb](https://github.com/HelloKS/ezTransWeb)