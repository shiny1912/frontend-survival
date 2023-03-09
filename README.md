# frontend-survival

GitBook of frontend-survival

## 1주차

**개발 환경 세팅**

*   .gitignore 파일 꼭 셋팅해주기

    .eslintignore파일도 셋팅&#x20;

```
/node_modules/
/dist/
/.parcel-cache/
```

* 터미널에서 typescript 빠르게 쓰기

```
npx ts-node
```

* ES Modules vs CommonJS
* NPM(Node Package Manager)

**Typescript**

* Node.js

ReactNode 처럼 레거시 코드도 있기 때문에 타입을 적용해줘야 한다.

Visual Studio Code의 자동 완성 + 실시간 오류 검사 기능이 있어서 편하다.

* Interface vs Type

Type이 더 오래된 개념이다.

* 타입 추론

모든 것을 작성하지 않아도 어느 정도 검사해 준다.

* Union Type

Union Type : 합집합.

type bool = true | false;

매개변수 제한시에도 유용하게 쓸 수 있다.

다른 타입을 적으면 빨간줄로 에러 체크해줌.&#x20;

* Optional Parameter

&#x20;Undefined로 파라미터를 받는 경우

function add(x:number, y?:number)&#x20;

* Intersection Type

type을확장한 것과 비슷한 개념

&#x20;type  Person = Human & Creature;

Interface의 merging개념을 활용하고 싶을 때가 아니라면 type을 쓰는 것이 코드가 더 일관성 있게 된다.

&#x20;

**React**

React 공식문서가 최근 함수 컴포넌트 위주로 update되었다.

리렌더링

State가 바뀔때 리렌더링한다.

부모가 리렌더링하면 자식도 리렌더링 가능하다.

Next.js나 Remix같은 케이스가 프레임워크에 더 가깝다.

&#x20;

**Jest**

expect로 assertion할 수 있다. Mocking도 쉽게 사용 가능.

&#x20;

Function add(x:number, y:number): number {

return x + y;

}

Test('숫자 더하기', () => {

&#x20;expect(add(1,2)).toBe(3);

});

Screen.getByText(\Hi\\); -> 정규표현식도 가능

&#x20;

**React Testing Library**

UI 테스트 라이브러리. 테스트 코드를 많이 작성하면 오히려 유지보수 할 때 로드가 더 많이 들어갈 수 있다.

&#x20;

&#x20;**Parcel**

&#x20;빌드 툴. Bundler 역할이다.

Npm i -D parcel-reporter-static-files-copy

.parcelrc 생성( json포맷)

&#x20;

빌드 + 정적 서버 실행

Npx parcel build

Npx servor ./dist

&#x20;

**ESLint**

스타일 통일, 잠재적 문제 발견

정적 프로그램 분석 : 시간이 짧음.

Npm run lint : 알아서 고쳐줌

Npm eslint --ext .tsx .

Trailing spaces

&#x20;



