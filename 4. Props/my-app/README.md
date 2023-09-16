# Props란?

리액트(React)에서 props는 "properties"의 약자로, 컴포넌트 간에 데이터를 전달하는 방법입니다. props는 부모 컴포넌트에서 자식 컴포넌트로 읽기 전용 데이터를 전달하는 데 사용됩니다. 

## 예시

```jsx
function Welcome(props) {
  return <h1>Hello, {props.name}!</h1>;
}

function App() {
  return <Welcome name="React" />;
}
```

위의 예제에서 App 컴포넌트는 name이라는 props를 Welcome 컴포넌트로 전달합니다. 그런 다음 Welcome 컴포넌트는 이 props를 사용하여 메시지를 렌더링합니다.

리액트에서 props는 컴포넌트 간의 상호작용 및 데이터 전달을 용이하게 만들어 줍니다. 다양한 데이터 타입 (문자열, 숫자, 배열, 객체, 함수 등)을 props로 전달할 수 있으며, 이를 통해 동적으로 UI를 구성하게 됩니다.
