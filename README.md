1..Describe an instance of prototypal inheritance in JavaScript?

cVb-miras her abyekt protip olarag bashqa bir abyektle ic baglantisi var.zincir prototip ozelliyi her hansi abyektin 
null deyeri verene qeder davam eder.
javascriptde obyekt dinamik konteyner her obyek daxilinde melumatlar saxliyir her hansi melumati almag ucun 
ilk oz daxiline baxir eyer yoxdusa obyektin prototipine muraciet elunur
null deyeri verene qeder bu davam eliyir
eyer obyekte yeni bir dyeer(meumat ) elave edilse bu yeni bir property sayilir yeni zincir mentiqi.
js-de her funcksiya abyekte (ozellik kimi)elave oluna biler. function icinde yazilan this o obyektin ozune istiqamet verir
prototipine yox
misal:
var o = {
  a: 2,
  m: function(){
    return this.a + 1;
  }
};

console.log(o.m()); // 3
//bu veziyyetde this o ya iware edir

var p = Object.create(o);
// 'p' - mirasci 'o'

p.a = 12; // 
console.log(p.m()); // 13
2..closures funksiya icindeki funksiyanin bir ustundeki funksiyaya tesiri demekdi.esas olan deyiuweni "var" nan teyin etmemekdir
function makeAdder(x) {
  return function(y) {
    return x + y;
  };
};

var add5 = makeAdder(5);
var add10 = makeAdder(10);

console.log(add5(2));  // 7
console.log(add10(2)); // 12

3..Can you use x === “object” to test if x is an object?
cVb-eyer 2 beraber olsaydi yalniz deyerini yoxluyardi eyer 3 bearber varsa hem data tipini hemde dyereini yoxluyur 
misal:
10=="10" trye  
10===10 trye
10==="10" false 
3bearber digerlerinnen ferqli olaarag hem data tipini hemde dyereini yoxluyur (repeted:()
4.What happens when you don’t declare a variable in Javascript?
cVb-deyiweni deklarasiya etmiyande deyiwen qlobal olur ister funksiya daxilinde istersede xaricinde 
ancag "var"nan teyin edilende qlobaldadisa qlobal funksiya daxilinidadise local olur 
5.What is the difference between == and === ?
cVb-iki beraber daxil edilen iki reqemin ya ededin biri birine beraber oldugunu yoxluyur (deyerinin builin qarwiligini)eyer trye dusa davam eliyir 
=== ise hem data tipi hemde bluilin deyerini yoxluyur her ikisi true du sa trye verir 
6.What datatypes are supported in Javascript?
cVb-javaScripte 6 data tipi var 
Boolean 
Null
Undefined 
Number 
String 
Symbol 
и Object
javaScript bawqa dillerden ferqi odurki yazilan datanin tipini ozu mueyyen edir yeniki onune girdiyiniz datanin tipini yazmag lazim olmur ancag bir xususiyeti daha var javaScript assinxron dildir yeni eyni vaxtda birnece datani qebul ede bilmir
7.What would “1”+2+3 and 1+2+“3” evaluate to, respectively?
cVb- bu veziyyetde ilk gosterilende 1-i string tipinde taniyacag ikinci gosterilendede 3-u string kimi aniyacag
yalniz - iwaresi olanda mecburi olarag cixma emeliyytibi heyata kecirir
8.Explain the concept of unobtrusive Javascript?
cVb-umumiyyetle html,css,js hamsi ayri yazilmalidi oxunurlug baximinnnan neyise qisa vaxtda tapib hell etmek baximinnan ancag inline yazlan stil deyiwikliyi daha suretlidi css de verilen deyiwiklik bele htnlde verilen deyiwikliye tesir elemir cunki htmlde verilen stuyle esas goturulur.
9.
