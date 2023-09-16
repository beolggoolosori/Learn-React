# 리액트에서의 이벤트

리액트(React)에서 이벤트는 DOM 요소에 설정되는 이벤트 핸들러를 통해 처리됩니다. 리액트의 이벤트 시스템은 기본 DOM 이벤트와 유사하게 작동하지만, 몇 가지 차이점이 있습니다.

## 예제

```jsx
class ButtonComponent extends React.Component {
  handleClick(e) {
    e.preventDefault();
    console.log('Button was clicked!');
  }

  render() {
    return (
      <button onClick={this.handleClick}>
        Click me
      </button>
    );
  }
}
```

이 예제에서 handleClick 메서드는 버튼이 클릭될 때 호출되는 이벤트 핸들러입니다. onClick은 버튼에 바인딩된 이벤트 핸들러입니다.
