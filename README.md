# CDK-SPA-Deploy
[![npm](https://img.shields.io/npm/dt/cdk-spa-deploy)](https://www.npmjs.com/package/cdk-spa-deploy)
[![Vulnerabilities](https://img.shields.io/snyk/vulnerabilities/npm/cdk-spa-deploy)](https://www.npmjs.com/package/cdk-spa-deploy)

단일 페이지 웹 사이트 (Angular / React / Vue)를 SSL / Cloudfront 뒤의 AWS S3에 5 줄의 코드로 쉽게 배포 할 수 있도록하는 AWS CDK Construct입니다.


## 설치 및 사용법

### Typescript
npm install --save cdk-spa-deploy

![cdk-spa-deploy example](https://raw.githubusercontent.com/nideveloper/cdk-spa-deploy/master/img/spadeploy.png)

### Python
pip install cdk-spa-deploy

![cdk-spa-deploy python example](https://raw.githubusercontent.com/nideveloper/cdk-spa-deploy/master/img/python.png)

## 고급 사용법

### Hosted Zone Name을 통해 부터 자동 배포

Route 53을 통해 도메인을 구매했고 이미 hosted zone이 있는 경우, 클라우드 프론트 뒤에 사이트를 배포하기위해 Hosted Zone Name을 사용할 수 있습니다. 이것은 SSL 인증서 및 모든 것을 처리할 수 있습니다.

![cdk-spa-deploy alias](https://raw.githubusercontent.com/nideveloper/cdk-spa-deploy/master/img/fromHostedZone.PNG)

### 사용자 정의 도메인 및 SSL 인증서

SSL 인증을위한 ARN과 alias routes를 Cloudfront로 전달할 수도 있습니다.

![cdk-spa-deploy alias](https://raw.githubusercontent.com/nideveloper/cdk-spa-deploy/master/img/cdkdeploy-alias.png)

### 암호화 된 S3 버킷

boolean 하나를 전달하여 SPA 배포에 웹 사이트 버킷을 암호화 할 수 있습니다.

![cdk-spa-deploy encryption](https://raw.githubusercontent.com/nideveloper/cdk-spa-deploy/master/img/encryption.PNG)

### 알려진 IP에 대한 접근 제한

boolean과 IP 주소 배열을 전달하면 접근 제한이 실시되고 사이트를 안전하게 보호할 수 있습니다.

![cdk-spa-deploy ipfilter](https://raw.githubusercontent.com/nideveloper/cdk-spa-deploy/master/img/ipfilter.png)

## 이슈 등록 / 기능 요청

https://github.com/nideveloper/CDK-SPA-Deploy
