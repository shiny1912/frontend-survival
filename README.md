# frontend-survival

GitBook of frontend-survival

## 1주차

1. 개발 환경 세팅
   *   .gitignore 파일 꼭 셋팅해주기

       .eslintignore파일도 셋팅

       &#x20;

       /node\_modules/

       /dist/

       /.parcel-cache/

       * Node.js
       * NPM(Node Package Manager)
       * ES Modules vs CommonJS
       * npx ts-node : 터미널에서 typescript 빠르게 쓰기
         *



2. Typescript

ReactNode 처럼 레거시 코드도 있기 때문에 타입을 적용해줘야 한다.

Visual Studio Code의 자동 완성 + 실시간 오류 검사 기능이 있어서 편하다.

* Interface vs Type

Type이 더 오래된 개념이다.

* 타입 추론

모든 것을 작성하지 않아도 어느정도 검사해 준다.

* Union Type

Union Type : 합집합.

type bool = true | false;

매개변수 제한시에도 유용하게 쓸 수 있다.

다른 타입을 적으면 빨간줄로 에러 체크해줌.&#x20;

* Optional Parameter

&#x20;Undefined로 파라미터를 받는 경우

function add(x:number, y?:number)&#x20;

* Intersection Type

확장한 것과 비슷한 개념

&#x20;type  Person = Human & Creature;

Interface의 merging개념을 활용하고 싶을 때가 아니라면 type을 쓰는 것이 코드가 더 일관성 있게 된다.

&#x20;

&#x20;



