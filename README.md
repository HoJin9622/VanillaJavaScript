# VanillaJavaScript

# local storage

자바스크립트의 작은 정보들을 저장해주는 공간

localstorage.getItem("name", value); - localstorage에 값을 불러옴.

localstorage.setItem("name"); - localstorage에 값을 저장.

자바스크립트는 local storage에 있는 모든 데이터를 string으로 저장.

# JSON

JavaScript Object Notation 의 준말

데이터를 전달할 때, 자바스크립트가 그걸 다룰 수 있도록 object로 바꿔주는 기능.

object와 string의 변환.

# JSON.stringify(object)

    JSON.sringify(object)

JSON.stringify는 자바스크립트 object를 string으로 바꿔준다.

# JSON.parse(string)

    JSON.parse(string)

JSON.parse는 자바스크립트 string을 object로 바꿔준다.

# filter 함수

filter는 array의 모든 아이템을 통해 함수를 실행하고, true인 아이템들만 가지고 새로운 array를 만든다.

# forEach

object.forEach(function) 을 실행하면 object에 대한 모든 것에 대해 function을 실행한다.

# Math 함수

    Math.random() * value

value 만큼의 값을 랜덤으로 준다.

    Math.floor(value)

소수점 나머지를 버림.

    Math.ceiling(value)

소수점 나머지 올림.

# 태그에 클래스 추가

    tag.classList.add("value");

원하는 tag에 value 클래스를 추가한다.

# 자바스크립트 객체 팁

    const coordsObj = {
        latitude,
        longitude
     };

객체의 필드와 값의 이름이 같으면 위와 같이 작성 가능

# CSS

transition: color 0.5s ease-in-out; - 컬러가 변경될때 0.5초 동안 서서히 바뀜

    const title = document.querySelector("#title");
    const CLICKED_CLASS = "clicked";

function handleClick() {  
title.classList.toggle(CLICKED_CLASS); // toggle 함수는 클래스를 체크해 있으면 add, 없으면 remove 해준다.
// title.classList.add(CLICKED_CLASS);
// title.classList.remove(CLICKED_CLASS);
}

function init() {
title.addEventListener("click", handleClick); // 자바스크립트 이벤트 찾기 : javscript dom event mdn
}
init();

/\* function handleResize() {
console.log("I have been resized");
}

window.addEventListener("resize", handleResize); \*/

/\* const title = document.querySelector("#title"); // document.getElementById("title");

title.innerHTML = "Hi! From JS";
title.style.color = "red";
console.dir(title);
document.title = "I own you now"; \*/

/\* function sayHello(name, age) {
return `Hello ${name} you are ${age} years`;
}

const greet = sayHello("Hojin", 23);
console.log(greet);

const calculator = {
plus: function(a, b) {
return a + b;
},
minus: function(a, b) {
return a - b;
},
mul: function(a, b) {
return a _ b;
},
div: function(a, b) {
return a / b;
},
route: function(a, b) {
return a \*\* b;
}
};
console.log(calculator.plus(5, 2));
console.log(calculator.minus(5, 2));
console.log(calculator.mul(5, 2));
console.log(calculator.div(5, 5));
console.log(calculator.route(5, 2)); _/

//camel case란 변수명을 언제나 소문자로 시작해서 중간에 스페이스가 필요하면 스페이스 대신에 대문자를 써준다.
//const what = "nico"; String type
//const wat = true; Boolean type
// const wat = 666; Number type
// const wat = 55.1; Float type
// const a : 바꿀 수 없는 변수, 바뀌어도 되는 변수 let
// 변수 첫 선언은 const 정말 필요할때만 let
// array 는 [] 로 해줌
// Object 는 {} 로 해줌
/\* const myInfo = {
name: "HoJin",
age: 23,
gender: "Male",
isHandsome: true
favMovies: ["Along the gods", "LOTR", "Oldbooy"],
favFood: [
{
name:"Kimchi",
fatty:false
},
{
name:"CheeseBurger",
fatty:true
}
]
};

console.log(myInfo.gender); \*/
// console << object, log << key,
