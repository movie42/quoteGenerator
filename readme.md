# Quote Generator  

> Udemy [JavaScript Web Projects: 20 Projects to Build Your Portfolio](https://www.udemy.com/course/javascript-web-projects-to-build-your-portfolio-resume/)

> Quote Generator는 외부 API를 사용하여 격언을 생성해주는 어플리케이션이다. [출처 : forismatic.com](https://forismatic.com/en/api/)

목적 : 20개의 프로젝트를 직접 해봄으로써 API 사용, DOM 조작 등을 실습해본다.  

## Quote Generator를 만들면서 복습해본것들.  
  

### CSS  

1. @import
   
   ``` css
   @import url("")
   ```

    구글에서 제공하는 웹 폰트를 간편하게 css로 불러올 수 있다. 폰트 외의 다른 많은 기능을 이런 방법으로 불러올 수 있을 것 같다.  

2. Animation  

    ``` css
    .loader{
        border: 16px solid #f3f3f3;
        border-top: 16px solid #38a1f3;
        border-radius: 50%;
        width: 120px;
        height: 120px;
        animation-name: spin;
        animation-duration: 2000ms;
        animation-iteration-count: infinite;
        animation-timing-function: linear;
    }

    @keyframes spin {
        from {
            transform: rotate(0deg);
        }
        to {
            transform: rotate(360deg);
        }
    }
    ```

    애니메이션은 사용자가 웹 페이지를 사용하면서 심리적으로 보다 안정감 있게 사용할 수 있도록 도울 수 있는 좋은 도구인것 같다. 애니메이션 이름을 지정하고 @keyframes를 가지고 애니메이션의 간단한 동작을 조작할 수 있다.  

### JavaScript

1. async /await  
    비동기 처리를 하는데 async/ await는 매우 유용한 방법이다. 콜백 함수나 promise를 사용하여 비동기 처리를 하는 것보다 훨씬 읽기 좋은 코드를 작성할 수 있게 도와준다.  

    출처 : Captain Pangyo powered by Jekyll  
    - [자바스크립트 비동기 처리와 콜백 함수](https://joshua1988.github.io/web-development/javascript/javascript-asynchronous-operation/#%EB%B9%84%EB%8F%99%EA%B8%B0-%EC%B2%98%EB%A6%AC-%EA%B7%B8%EA%B2%8C-%EB%AD%94%EA%B0%80%EC%9A%94)  
    - [자바스크립트 Promise 쉽게 이해하기](https://joshua1988.github.io/web-development/javascript/promise-for-beginners/#promise%EA%B0%80-%EB%AD%94%EA%B0%80%EC%9A%94)  
    - [자바스크립트 async와 await](https://joshua1988.github.io/web-development/javascript/js-async-await/#async--await%EB%8A%94-%EB%AD%94%EA%B0%80%EC%9A%94)

2. try and catch  
    에러 핸들링을 하는데 사용되는 방법이다. finally도 뒤에 더 붙일 수 있다.  

    2-1. fetch  
    외부 데이터를 불러올 때 사용한다. 나중에 Axios를 사용하면 fetch보다 편하게 외부 데이터를 불러올 수 있다.  

3. classList.add, classList.remove  
   classList는 HTML에 class를 추가하는 방법중에 하나다. css로 class에 대한 정의를 내려놓고 특정 조건에서 (예 : 버튼 클릭) class가 추가되고 제거되는 것을 통해 화면을 가리거나 창을 띄우거나 하는 동작을 추가할 수 있다. 버튼에서 toggle을 사용하기도 한다.  

