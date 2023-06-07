## React 입문

## 목차
- [React 입문](#react-입문)
- [목차](#목차)
- [React란](#react란)
- [React 라이프사이클](#react-라이프사이클)

## React란
* MVC 패턴 중 View에 해당하는 라이브러리 
* Vortual DOM 을 이용한 렌더링
* JSX 문법 사용
* Vue, Anglar와 다르게 단방향 데이터 바인딩 사용
* Componenet 기반의 아키텍쳐

## React 라이프사이클

### Mount
* 컴포넌트의 리액트 인스턴스가 생성되어 DOM에 추가될 때 발생

Mount 시 메소드 호출 순서

* constructor()
* static getDerivedStateFromProps()
* render()
* componentDidMount() 
<br><br>

### Upadate
* props나 state가 변경될 때 발생

Update 시 메소드 호출 순서

* static getDerivedStateFromProps()
* shouldComponentUpdate()
* render()
* getSnapshotBeforeUpdate()
* componentDidUpdate()
<br><br>

### Unmount
* 컴포넌트가 DOM에서 제거될 때 발생

Unmount 시 메소드 호출 순서

* componentWillUnmount()
