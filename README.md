# 따라하는 리액트 테스트

## 1. Testing을 위한 설정 및 준비

-   Jest-Dom
-   Testing Library
-   ESLint
-   Prettier

## 2. 테스트를 하는 이유

### 테스트를 하는 이유

간단하게 더 안정적인 앱을 만들기 위해 여러가지 테스트를 한다
테스트모듈이 없다면 일일이 버그가 발생할 때마다 UI쪽 문제인지 DB의 문제인지 등 원인을 찾아야 한다.

### 얻는 이점

1. 디벅이 시간 단축
2. 안정성
3. 재설계 시간의 단축, 추가로 무언가를 더 구현해야 할 때 용이함

## 3. React Testing Library

React Testing Library는 React의 구성 요소 작업을 위한 API를 추가하여 DOM Testing Library 위에 구축된다.
DOM Testing Library란 DOM 노드 (Node)를 테스트하기 위한 매우 가벼운 솔루션
CRA로 생성된 프로젝트는 React Testing Library를 `즉시` 지원함.
그렇지 않은 경우에는 npm으로 추가 가능

```
npm instasll --save-dev @testing-library/react
```

리액트 컴포넌트를 테스트하는 가벼운 솔루션이다.

### Enzyme

-   구현 주도 테스트
-   A와 B컴포넌트 사이에 어떻게 상태가 흐르고 어떻게 교환하는지를 중점

### React Testing Library

-   행위 주도 테스트
-   사용자 입장에선 어떤 상태가 교환되는지 알 필요가 없다(모른다).
    사용자가 어떠한 행위를 가했을 때 어떠한 일이 일어나는지를 위주로 테스트
