# QuickStart

좋은 도구를 사용하면 모든 것을 손으로 다룬 것보다 응용프로그램을 보다 빠르고 쉽게 유지관리 할 수 있습니다.
Angular CLI는 프로젝트를 만들고 파일을 추가하며 테스트, 번들링 및 배포와 같은 다양한 개발 작업을 수행할 수 있는 명령 줄 인터페이스 도구입니다.
이 가이드의 목표는 모든 Angular 프로젝트에 도움이 되는 Style Guide 권장사항을 준수하면서 Angular CLI를 사용하여 TypeScript에서 간단한 Angular 응용프로그램을 작성하고 실행하는 것입니다.
이 장의 끝 부분에서는 CLI를 사용한 개발에 대한 기본적인 이해와 이 문서 샘플과 실제 응용프로그램의 기초를 얻을 수 있습니다.
그리고 예제를 다운로드 할 수도 있습니다.

## 1단계. 개발환경 설정
우선 개발 환경을 설정합니다. Node.js와 npm을 설치합니다.
터미널/콘솔 창에서 "node -v", "npm -v" 를 실행하여 적어도 node 6.9.x, npm 3.x.x를 실행 중인지 확인합니다. 이전 버전에서는 오류가 발생하지만 최신 버전에서는 문제가 없습니다.
그런 다음 Angular CLI를 전역적(globally)으로 설치합니다.

```
npm install -g @angular/cli
```

## 2단계. 새 프로젝트 생성
터미널 창을 엽니다. 다음 명령어를 실행하여 새로운 프로젝트와 응용프로그램 뼈대를 생성합니다. 새로운 프로젝트를 설정하는데 시간이 걸립니다.

```
ng new my-app
```

## 3단계. 응용프로그램 Serve
생성된 프로젝트 디렉토리로 이동하여 서버를 시작합니다. "ng serve" 명령어로 서버를 시작하고 파일을 감시하며 해당 파일을 변경할 때 응용프로그램을 다시 빌드합니다. "--open(또는 -o)" 옵션을 사용하면 브라우저에 http://localhost:4200/ 가 자동으로 열립니다.

```
cd my-app
ng serve --open
```

다음과 같은 메시지를 보실 수 있습니다.

## 4단계. 첫번째 Angular 컴포넌트 수정
CLI는 첫번째 Angualr 컴포넌트를 생성합니다. 이것은 "app-root"라 불리우는 root 컴포넌트입니다.
./src/app/app.component.ts에서 찾을 수 있습니다.
컴포넌트 파일을 열어 title 속성을 "Welcome to app!!"에서 "Welcome to My First Angular App!!"로 변경합니다.

src/app/app.component.ts
```
export class AppComponent {
    title = 'Welcome to My First Angular App!!';
}
```

브라우저는 수정된 제목으로 자동으로 다시 로드됩니다. 
src/app/app.component.css를 열고 컴포넌트에 style을 지정합니다.

src/app/app.component.css
```
h1 {
    color: #369;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 250%;
}
```