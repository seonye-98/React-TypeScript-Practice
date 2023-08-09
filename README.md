# React-TypeScript-Practice

React에 TypeScript를 적용하는 연습 프로젝트

# 리액트 세팅 방법

1. create-react-app 설치

```ts
npm install -g create-react-app
```

2. TypeScript를 활용한 React 환경 구축

```ts
npx create-react-app 디렉토리명 --template typescript
```

현재 디렉토리에 생성하고 싶다면 디렉토리명에 . 을 넣어주면 된다.

> npm대신 npx를 쓰는이유?
> 글로벌 모듈을 설치하지 않기 위함이다. 한 번 설치면 끝나는데 왜 좋은 방법이 아닐까?

1. 모듈이 업데이트 되었는지 안되었는지 확인이 불가능하다.
2. 업데이트를 진행했을 때 변동사항이 생겨 다른 프로젝트에도 영향을 끼칠 수 있다.
3. create-react-app 같은 보일러플레이트에는 치명적이다.
   -> 리액트 프로젝트 생성 도구인 create-react-app 같은 모듈의 경우, 변경사항이 잦기 때문에 항상 최신 버전을 유지해 주는 것이 좋다.

**해결책 -> npx**
글로벌 모듈을 로컬에 저장하지 않고, 매번 최신 버전의 파일만을 임시로 불러와 실행 시킨 후에, 그 파일은 없어지는 방식으로 모듈을 돌아가게 한다.

결론 : 프로젝트의 의존성 패키지를 설치하고 빌드하는 경우 npm, 일회성으로 도구를 실행하거나 최신 버전의 패키지를 사용해야 하는 경우 npx를 사용한다.

[출처](https://ljh86029926.gitbook.io/coding-apple-react/undefined/npm-npx)
