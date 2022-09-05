# 반응형 웹페이지 구현

### [프로젝트 목표]

- HTML을 통한 웹 페이지 마크업 이해

- CSS 라이브러리의 이해와 활용
- Bootstrap 컴포넌트 및 Grid system을 활용한 반응형 레이아웃 구성

### [요구사항]

#### 01_nav_footer

- **Modal**

  - 버튼으로 만들기 

    ```html
    <li><button type="button" class="btn btn-link text-white text-decoration-none" data-bs-toggle="modal" data-bs-target="#exampleModal">Login</button></li>
    ```

  - `<a>`로 만들기

    ```html
    <li><a href="./03_community.html" class="text-white text-decoration-none" data-bs-toggle="modal" data-bs-target="#exampleModal">Login</a></li>
    ```

  - `data-bs-toggle="modal" data-bs-target="#exampleModal"` : modal 로 연결해 주는 제일 중요한 내용.

  - `<a>`를 수정하려고 했으나, 위의 내용을 몰라서 버튼 스타일을 변경하는 방식으로 작성했다.

- **Collapse**

  - 컨텐츠를 표시하고 숨기는데 사용한다.

  - 연결방법은 두가지 이다.

  - 네비게이션 `三` 버튼 눌렀을 때 네비게이션바 아래로 메뉴가 나열되도록 할 때 이용했다. 

  - 연결방법은 두가지 이다.

    - `<a>`를 이용한 연결

      ```html
      <a class="btn btn-primary" data-bs-toggle="collapse" href="#collapseExample" role="button" aria-expanded="false" aria-controls="collapseExample">
          Link with href
        </a>
      ```

    - button을 이용한 연결

      ```html
      <button class="btn btn-primary" type="button" data-bs-toggle="collapse" data-bs-target="#collapseExample" aria-expanded="false" aria-controls="collapseExample">
          Button with data-bs-target
        </button>
      ```

**[ 좌측 상단 로고 고정]** 

- Grid로 넣어서 만들었더니 화면이 줄어들면 로고가 찌그러졌다.

- 다른 부분과 크게 영향이 없는 위치라고 생각해 Float를 이용했다.

  ```html
  <img src="images/logo.png" style="height: 50px; margin-right: 30px;" class="float-start" alt="Logo Image">
  ```

#### ~~02_home~~

#### 03_community

- **Section Aside**
  - 명세에 `1/6만큼의 너비` ,`5/6만큼의 너비`를 보고 Grid를 이용하면 되겠다고 생각했다.

- **Table**

  ```html
  <table class="table">
    <thead>
      <tr>
        <th scope="col">#</th>
        <th scope="col">First</th>
        <th scope="col">Last</th>
        <th scope="col">Handle</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th scope="row">1</th>
        <td>Mark</td>
        <td>Otto</td>
        <td>@mdo</td>
      </tr>
  ```

  



