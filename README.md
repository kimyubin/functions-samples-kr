# Firebase용 클라우드 기능 샘플 라이브러리

이 저장소는 [Firebase용 클라우드 기능](https://firebase.google.com/features/functions)의 일반적인 사용 사례를 보여주는 샘플 컬렉션을 포함하고 있습니다.

샘플은 **Node** (2세대), **Python** (2세대), 그리고 Node (1세대)에 대해 제공됩니다.

> 주의: Firebase용 클라우드 기능의 Python 지원은 공개 미리보기입니다. 이는 기능이 하위 호환이 아닌 방식으로 변경될 수 있음을 의미합니다. 미리보기 버전은 SLA 또는 중단 정책의 적용을 받지 않으며 제한적이거나 전혀 지원되지 않을 수 있습니다.

### Firebase용 클라우드 기능이란?

클라우드 기능은 JavaScript 또는 Python 코드를 실행할 수 있는 호스팅되고 개인적이며 확장 가능한 Node.js 환경입니다. [Firebase용 클라우드 기능](https://firebase.google.com/features/functions)은 다른 Firebase 기능에서 제공하는 기능을 호출하고 이벤트에 응답하는 코드를 작성할 수 있게 하여 Firebase 플랫폼과 통합됩니다.

## 전제 조건

> 모든 샘플은 배포를 위한 Blaze 종량제 요금제를 요구합니다. [요금](https://firebase.google.com/pricing#cloud-functions) 관련 내용은 더 알아보세요.

Firebase용 클라우드 기능을 시작하는 방법은 [시작 가이드](https://firebase.google.com/docs/functions/get-started)를 살펴보거나 [퀵스타트 샘플](/Node/quickstarts)을 시도하고 [문서](https://firebase.google.com/docs/functions)를 참고하시기 바랍니다.

<a name="quickstarts"></a>
## 퀵스타트

각 클라우드 기능 트리거 유형에 대한 최소 샘플입니다.

### 퀵스타트: Firestore용 대문자로 변환기

- [Node 2세대](/Node/quickstarts/uppercase-firestore/)
- [Python](/Python/quickstarts/uppercase-firestore/)
- [Node 1세대](/Node-1st-gen/quickstarts/uppercase-firestore/)

이 퀵스타트 샘플은 **Firestore 이벤트**에 의해 트리거되는 **클라우드 기능**의 사용을 보여줍니다. 이 기능은 Firestore에 기록된 메시지 텍스트를 대문자로 변환합니다.

### 퀵스타트: 호출 가능한 함수로 숫자 더하기 및 텍스트 정제하기

- [Node 2세대](/Node/quickstarts/callable-functions/)
- [Python](/Python/quickstarts/callable-functions)
- [Node 1세대](/Node-1st-gen/quickstarts/callable-functions/)

### HTTPS 트리거 퀵스타트: 시간 서버

- [Node 2세대](/Node/quickstarts/https-time-server/)
- [Python](/Python/quickstarts/https-time-server/)
- [Node 1세대](/Node-1st-gen/quickstarts/https-time-server/)

이 퀵스타트 샘플은 **HTTPS 요청**에 의해 트리거되는 **클라우드 기능**의 사용을 보여줍니다. 이 기능은 현재 서버 시간을 반환하며 날짜 및 시간 형식을 설정할 수 있습니다.

### 퀵스타트: Realtime Database용 대문자로 변환기

- [Node 2세대](/Node/quickstarts/uppercase-rtdb/)
- [Python](/Python/quickstarts/uppercase-rtdb/)
- [Node 1세대](/Node-1st-gen/quickstarts/uppercase-rtdb/)

이 퀵스타트 샘플은 **Realtime Database 이벤트**에 의해 트리거되는 **클라우드 기능**의 사용을 보여줍니다. 이 기능은 Realtime Database에 기록된 메시지 텍스트를 대문자로 변환합니다.

### 호스팅 트리거된 HTTPS 함수 퀵스타트: 빅 벤

- [Node 1세대](/Node-1st-gen/quickstarts/big-ben/)

이 퀵스타트는 Firebase Hosting URL을 통해 트리거되는 HTTPS 트리거로 **클라우드 기능**을 사용하는 방법을 보여줍니다. 이 기능은 하루 시간에 따라 반복적으로 "BONG"을 표시합니다.

### 클라우드 스토리지 트리거 퀵스타트: 썸네일 생성기

- [Node 2세대](/Node/quickstarts/https-time-server/)
- [Python](/Python/quickstarts/https-time-server/)
- [Node 1세대](/Node-1st-gen/quickstarts/https-time-server/)

이 퀵스타트 샘플은 **Firebase Storage 이벤트**에 의해 트리거되는 **클라우드 기능**의 사용을 보여줍니다. 이 기능은 업로드된 이미지의 썸네일을 생성합니다.

### 인증 트리거 퀵스타트: 환영 이메일

> 인증 사용자 생성 및 삭제 트리거는 아직 2세대 기능에서 지원되지 않습니다.

- [Node 1세대](/Node-1st-gen/quickstarts/email-users/)

이 퀵스타트 샘플은 **Firebase Auth 이벤트**에 의해 트리거되는 **클라우드 기능**의 사용을 보여줍니다. 이 기능은 사용자 계정이 생성될 때(또는 사용자가 처음으로 Identity Provider를 통해 로그인할 때) 환영 이메일을 전송하고, 사용자 계정이 삭제될 때는 작별 이메일을 전송합니다.

### 인증 차단 트리거 빠른 시작: 사용자 상태 검증 및 확인

- [Node 2세대](/Node/quickstarts/auth-blocking-functions/)
- [Python](/Python/quickstarts/auth-blocking-functions/)
- [Node 1세대](/Node-1st-gen/quickstarts/auth-blocking-functions/)

이 빠른 시작은 **인증 차단 기능**을 사용하여 사용자가 로그인할 수 있도록 하기 전에 이메일을 검증하고, Firestore에서 사용자 차단 목록에 사용자가 포함되어 있는지를 확인하는 방법을 보여줍니다.

### PubSub 트리거 빠른 시작: Hello World

- [Node 2세대](/Node/quickstarts/pubsub-helloworld/)
- [Python](/Python/quickstarts/pubsub-helloworld/)
- [Node 1세대](/Node-1st-gen/quickstarts/pubsub-helloworld/)

이 빠른 시작 샘플은 **PubSub 이벤트**에 의해 트리거되는 **Cloud Functions**를 사용하는 방법을 보여줍니다. 함수는 Hello World 메시지의 PubSub 페이로드를 기록합니다.

### 테스트 실험실 트리거 빠른 시작: 매트릭스가 완료될 때 로그 기록

- [Node 2세대](/Node/quickstarts/testlab-matrix-completed/)
- [Python](/Python/quickstarts/testlab-matrix-completed/)

### Firebase 알림 트리거 빠른 시작: 크래시 보고서를 Discord에 전송하기](/2nd-gen/alerts-to-discord/)

- [Node 2세대](/Node/alerts-to-discord/)
- [Python](/Python/alerts-to-discord/)
- Node 1세대: 지원되지 않음

Firebase 알림에 기반하여 함수를 트리거하고, 경고에 대한 정보를 Discord 서버의 채널에 전송합니다.

### 사용자 정의 이벤트: 이미지 메타데이터 저장

- [Node 2세대](/Node/quickstarts/custom-events/)
- [Python](/Python/quickstarts/custom-events)
- Node 1세대: 지원되지 않음

확장 프로그램에서 전송된 이벤트를 기반으로 함수를 트리거하는 방법을 배웁니다.

### 단위 테스트

- [Jest로 테스트하기](/Node/test-functions-jest/)
    - [Jest 및 TypeScript로 테스트하기](/Node/test-functions-jest-ts/)
- [Mocha로 테스트하기](/Node/test-functions-mocha/)

<a name="environment"></a>
## 개발 보일러플레이트

Firebase CLI는 JavaScript 또는 TypeScript를 사용하여 Cloud Functions의 샘플 코드를 생성합니다.

### Handlebars 템플릿 및 사용자 세션을 사용한 서버 측 생성 페이지

- [Node (1세대)](/Node-1st-gen/template-handlebars)

이 샘플은 [HandlebarsJs](http://handlebarsjs.com/) 템플릿 시스템을 사용하여 서버 측에서 생성된 HTML 페이지를 제공하고, Firebase ID 토큰을 항상 `__session` 쿠키로 전달하여 사용자별 콘텐츠를 제공하는 방법을 보여줍니다.

<a name="image"></a>
## 이미지 처리

Cloud Functions를 사용하여 이미지를 처리하거나 분석하는 방법을 보여주는 몇 가지 샘플입니다.

### 이미지 메이커

- [Node (1세대)](/Node-1st-gen/image-maker)

이 샘플은 Cloud Functions와 호스팅을 통해 스파크라인 또는 구형 차트와 같은 다양한 맞춤형 이미지를 생성하고 클라이언트에 제공하는 방법을 보여줍니다.
HTTP 트리거를 사용합니다.

### 업로드 후 이미지 변환

- [Node (1세대)](/Node-1st-gen/convert-images)

Firebase Storage에 업로드된 이미지를 자동으로 JPEG로 변환하는 방법을 보여줍니다. 
Firebase Storage 트리거를 사용합니다.

### 공격적인 이미지 조정

- [Node (1세대)](/Node-1st-gen/moderate-images/)

Firebase Storage에 업로드된 공격적인 이미지를 자동으로 조정하는 방법을 보여줍니다. Google Cloud Vision API를 사용하여 공격적인 이미지를 감지하고 ImageMagick을 사용하여 이러한 이미지를 흐리게 처리합니다.
Firebase Storage 트리거를 사용합니다.

### 이미지 메타데이터 추출

- [Node (1세대)](/Node-1st-gen/exif-images/)

Firebase Storage에 업로드된 이미지에서 메타데이터를 자동으로 추출하는 방법을 보여줍니다.
Firebase Storage 트리거를 사용합니다.

### 작업 큐: API에서 이미지 백업

- [Node 2세대](/Node/taskqueues-backup-images/)
- [Python](/Python/taskqueues-backup-images/)

모든 트래픽을 비율 제한 API로 조절하기 위해 작업 큐를 사용하는 방법을 살펴봅니다.

<a name="rtdb"></a>
## Firebase 실시간 데이터베이스 데이터 일관성

이 샘플들은 자녀 수를 유지하거나, 노드 자식 수의 최대치를 갖고, 오래된 데이터를 정리하는 등 자동 데이터 일관성을 구현하는 방법을 보여줍니다.

### LastModified Firebase 실시간 데이터베이스 추적

- [Node (1세대)](/Node-1st-gen/lastmodified-tracking)

Firebase 데이터베이스(또는 하위 집합)가 마지막으로 수정된 시간을 추적합니다.
실시간 데이터베이스 트리거를 사용합니다.

### Firebase Database 자식 노드 수

- [Node (1세대)](/Node-1st-gen/child-count)

Firebase Database 요소의 자식 노드 수를 추적하여 클라이언트가 자식 수를 사용해 결과를 필터링하거나 정렬할 수 있게 합니다. 이는 소셜 미디어를 통해 공유되는 "좋아요" 또는 "팔로워" 수를 추적하는 데 유용할 수 있습니다. Realtime Database 트리거를 사용합니다.

### 자식 노드 수 제한

- [Node (1세대)](/Node-1st-gen/limit-children)

자식 노드 수가 특정 임계값 이하로 유지되도록 합니다. 이는 로그 또는 채팅 기록의 라인 수를 주어진 숫자 이하로 제한하는 데 유용할 수 있습니다. Realtime Database 트리거를 사용합니다.

### 목록에서 오래된 항목 제거

- [Node (1세대)](/Node-1st-gen/delete-old-child-nodes)

이 샘플은 Firebase Database 목록에서 2시간 이상 된 자식 노드를 제거하는 방법을 보여줍니다. 이는 컬렉션에서 구식 항목을 제거하는 데 유용할 수 있습니다. Realtime Database 트리거를 사용합니다.

<a name="other"></a>
## 다른 일반적인 사용 사례 해결

### FCM 알림 전송

- [Node (1세대)](/Node-1st-gen/fcm-notifications)

이 샘플은 사용자가 새로운 팔로워를 얻었을 때 Realtime Database로 트리거된 함수에서 Firebase Cloud Messaging (FCM) 알림을 보내는 방법을 보여줍니다. 샘플에는 FCM 알림을 체험할 수 있는 웹 UI도 포함되어 있습니다. Realtime Database 트리거를 사용합니다.

### Google Assistant가 주어진 숫자의 서수를 말하기

- [Node (1세대)](/Node-1st-gen/assistant-say-number)

이 샘플은 Cloud Functions에서 호스팅된 Actions SDK를 사용하여 Google Home/Assistant를 위한 액션을 생성하는 방법을 보여줍니다. 샘플 액션은 사용자가 숫자를 말하도록 요청하고 해당 숫자의 서수를 읽어줍니다. HTTP 트리거를 사용합니다.

### 인증된 JSON API

- [Node (1세대)](/Node-1st-gen/authenticated-json-api)

이 샘플은 특정 Firebase 사용자에 대해서만 데이터 접근을 허용하기 위해 JSON API 접근을 인증하는 방법을 보여줍니다. HTTP 트리거를 사용합니다.

### 허가된 HTTP 엔드포인트

- [Node (1세대)](/Node-1st-gen/authorized-https-endpoint)

이 샘플은 앱의 Firebase 사용자만 사용하도록 HTTPS 기능을 제한하는 방법을 보여줍니다. 유효한 Firebase ID 토큰을 Bearer 토큰으로 HTTP 요청의 `Authorization` 헤더 또는 `__session` 쿠키에 전달하는 사용자만 기능을 사용할 수 있습니다. ID 토큰 검사는 ExpressJs 미들웨어로 수행되며, 해당 미들웨어는 Express 요청 객체에 디코딩된 ID 토큰을 전달합니다. HTTP 트리거를 사용합니다.

### 제3자 인증 제공자로 인증

[Okta](/Node-1st-gen/okta-auth), [LinkedIn](/Node-1st-gen/linkedin-auth), [Spotify](/Node-1st-gen/spotify-auth), [Instagram](/Node-1st-gen/instagram-auth), 또는 [기본 인증](/Node-1st-gen/username-password-auth)

제3자 로그인 메커니즘으로 인증하고 Firebase 사용자 정의 인증 토큰을 생성하며, 사용자의 프로필을 업데이트하고 Firebase를 인증하는 방법을 보여줍니다. HTTP 트리거를 사용합니다.

### GitHub 커밋을 Slack 채널에 게시

- [Node (1세대)](/Node-1st-gen/github-to-slack)

HTTPS 트리거된 기능을 사용하여 GitHub 커밋을 Slack 채널에 자동으로 게시하는 방법을 보여줍니다.

### [Stripe](/Node-1st-gen/stripe) 또는 [Paypal](/Node-1st-gen/paypal)로 고객 생성 및 청구

Firebase Auth와 Realtime Database를 Stripe의 Stripe Node.js 라이브러리를 통해 통합하는 방법과 Paypal을 통해 고객에게 청구하기 위한 HTTP 엔드포인트를 생성하는 방법을 보여줍니다.

### 텍스트 검열

- [Node (1세대)](/Node-1st-gen/text-moderation)

사용자 입력 텍스트에서 나쁜 단어를 검열하는 방법을 보여줍니다. 이는 사용자 이름, 채팅 또는 포럼 메시지를 검열하는 데 사용될 수 있습니다. Realtime Database 트리거를 사용합니다.

### 이메일 확인

- [Node (1세대)](/Node-1st-gen/email-confirmation)

사용자가 메일링 리스트에 구독한 후 이메일 확인을 전송합니다. Realtime Database 트리거를 사용합니다.

### 자동 메시지 번역

- [Node (1세대)](/Node-1st-gen/message-translation)

Google Translate API를 통합하여 여러 언어 간 자동 텍스트 번역을 수행합니다. 언어 코드는 Firebase에 저장되어 실시간 변경이 가능합니다. Realtime Database 트리거를 사용합니다.

### 자동 URL 단축기

- [Node (1세대)](/Node-1st-gen/url-shortener)

Bit.ly API를 통합하여 데이터베이스에 추가되는 URL을 자동으로 단축합니다. Realtime Database 트리거를 사용합니다.

### [Realtime Database](/Node-1st-gen/fulltext-search) 또는 [Firestore](/Node-1st-gen/fulltext-search-firestore) 전체 텍스트 검색

호스팅된 검색 서비스를 사용하여 Firebase Database 데이터 또는 Firestore 문서에서 전체 텍스트 검색을 활성화합니다. Realtime Database 또는 Firestore 트리거를 사용합니다.

### 사용자 데이터 정리

- [Node (1세대)](/Node-1st-gen/user-data-cleanup)

사용자가 Firebase 계정을 삭제할 때 Realtime Database에서 모든 관련 사용자 데이터를 삭제합니다. Auth 트리거를 사용합니다.
**이 코드는
https://github.com/firebase/user-data-protection에 있는 자체 리포지토리로 이동했습니다.**

### 데이터를 Google 스프레드시트로 내보내기

- [Node (1세대)](/Node-1st-gen/google-sheet-sync)

이 샘플은 Firebase 데이터베이스에 작성된 새로운 데이터를 Google 시트에 동기화하는 방법을 보여줍니다. Google API 접근을 위한 Oauth2 토큰을 얻고 저장하며 사용하는 방법을 포함합니다. HTTPS 트리거와 Realtime Database 트리거를 사용합니다.

### 데이터를 Big Query로 내보내기

- [Node (1세대)](/Node-1st-gen/bigquery-import)

Firebase Database 요소를 BigQuery로 자동으로 복사합니다. 이는 로그 분석을 위한 예를 들면 유용할 수 있습니다. Realtime Database 트리거를 사용합니다.

### Firebase Database에 쓰기 시 Webhook 요청

- [Node (1세대)](/Node-1st-gen/minimal-webhook)

Firebase Database에 쓰기를 하면 콜백 URL(웹후크)에 요청이 트리거됩니다. 수정된 데이터의 내용이 웹후크로 전송됩니다. Realtime Database 트리거를 사용합니다.

### 앱 업데이트 시 사용자에게 설문 조사 전송

- [Node (1세대)](/Node-1st-gen/survey-app-update)

이 샘플은 앱을 업데이트한 사용자에게 설문조사를 전송하는 방법을 보여줍니다. 앱 업데이트는 Firebase Analytics 이벤트를 사용하여 감지됩니다. Analytics 트리거를 사용합니다.

### 구매 완료한 사용자에게 쿠폰 전송

- [Node (1세대)](/Node-1st-gen/coupon-on-purchase)

이 샘플은 막 구매한 사용자에게 쿠폰을 보내는 방법을 보여줍니다. 다음 구매 시 10% 할인! Analytics 트리거를 사용합니다.

### 비활성 사용자 계정 주기적으로 삭제

- [Node (1세대)](/Node-1st-gen/delete-unused-accounts-cron)

지난 한 달 동안 로그인하지 않은 사용자의 계정을 주기적으로 삭제합니다. HTTPS 트리거를 사용합니다.

### 개발자 동기 부여

- [Node (1세대)](/Node-1st-gen/developer-motivator)

이 샘플은 앱이 사용자를 얻거나 잃을 때마다 개발자 기기에 Firebase Cloud Messaging (FCM) 알림을 전송하는 방법을 보여줍니다. Analytics 트리거를 사용합니다.

### 오디오 파일 변환

- [Node (1세대)](/Node-1st-gen/ffmpeg-convert-audio)

이 샘플은 ffmpeg / fluent-ffmpeg를 사용하여 Cloud Storage에 업로드된 오디오 파일을 자동으로 FLAC 파일 형식으로 변환합니다. 오디오 채널은 단일이며 샘플링 주파수는 16000hz입니다. Storage 트리거를 사용합니다.

### Firestore의 Presence

- [Node (1세대)](/Node-1st-gen/presence-firestore)

Firestore와 Realtime Database를 함께 활용하여 사용자들의 간단한 온라인/오프라인 상태 표시기를 구축합니다. Realtime Database 트리거를 사용합니다.

### Firebase ML에 모델 게시

- [Node (1세대)](/Node-1st-gen/publish-model)

Firebase Storage에 업로드된 각 TensorFlow Lite 파일에 대해 자동으로 Firebase ML에 모델을 게시합니다.

### YouTube 채널에 대한 정보 가져오기 

- [Node (1세대)](/Node-1st-gen/youtube)

이 샘플은 YouTube Data API를 쿼리하는 방법을 보여줍니다. HTTPS 트리거를 사용합니다.

## 기여하기

프로젝트에 기여하고 싶습니다. 기여하기 전에 [기여자 가이드](CONTRIBUTING.md)를 읽어 주세요.

## 라이센스

© Google, 2015-2023. [Apache-2](LICENSE) 라이센스에 의해 라이센스가 부여됩니다.

## 빌드 상태

[![작업 상태][gh-actions-badge]][gh-actions]

[gh-actions]: https://github.com/firebase/functions-samples/actions
[gh-actions-badge]: https://github.com/firebase/functions-samples/workflows/CI%20Tests/badge.svg

