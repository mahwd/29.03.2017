# 29.03.2017
1. Describe an instance of prototypal inheritance in JavaScript?
-  her bir objectin private prototype var . O da yaradildigi constructordi.  Object constructorla create olunmayibsa, onun prototype Object olur.  Object create olundugu constructordan inheritance alir. Hemin object de basqa bir objectin prototipi olursa hamisi arasinda prototypal inheritance yaranir . Aralarindaki nesil elaqesi de prototype chain adlanir. Baba, ogul, neve ve s. arasindaki nesillik elaqesini prototypal inheritance-a misal gostere bilerem.  Prototype chainin asagisindaki olan objectler ucun ancestorlarinin method ve propertileri elcatandi.

2. What are closures and how are they used? 
- closure object icine gomulu funksiyadir. Buna method() deyirik. Eventhandler(), callback()  closure mentiqi ile yaziriq. Closure islenmesi data security (data abstraction) temin edir. 
Example : 
var someObject = {
someMethod : function (ad,soyad){ 
	console.log(“Salam “+ad+” “+soyad)
}
}

someObject.someMethod(‘Rehim’ , ’Rehimli’);

someMethod()  burda closure du

3. Can you use x === “object” to test if x is an object?
- Yox amma 	
If ((typeof x )=== “object”) statement ile eliye bilerik

4. What happens when you don’t declare a variable in Javascript?
- variable teyin olunanda yaddasda onun ucun flag acilir ve dinamik yer ayrilir.



5. What is the difference between == and === ?
- 	cut = lik ayri data typelari da muqayise edir === ise data tipinin de eyniliyini yoxlayir.
a = 5;
b = “5”
a == b    true
a===b   false

6. What datatypes are supported in Javascript?
- js de esas 7 data tipi var:
-Boolean
-Null
-Undefined
-Number (integer float long so on)
-String
-Symbol (char)
-Object

7. What would “1”+2+3 and 1+2+“3” evaluate to, respectively?
number + number = number // string + number = string // sting + string = string
@ “1”+5 = 123
@ 3+”3” = 33

8. Explain the concept of unobtrusive Javascript?
- sade javascript html taglarine gomulen js kodlaridi 
Meqsedi js kodlari run olunmasini garantilemekdi daha dogrusu browser js kodunu desteklemedikde bele sehifenin iwlek veziyyetde olmasidir.
Example :
<a href=”javascript:window.open(‘http://www.google.com’)”>Click me</a>

9. What is the difference between a null value and an undefined value?
- data tipleri ayridi , null objectdi ,undefined undefineddi
Typeof null = “object”
Typeof undefined= “undefined”
Null ancaq assign oluna bilen data typedi . Null dedikde yeni a=null; dedikde variable -a bos bir object assign etmis oluruq;
typeof a = “object”
a = “null” 

10. Which conditional statements will JavaScript support?
- 2 nov sert operatoru var 
@ condition ? expr1 : expr2
condition  wert
expr1  wert odenen hal
exp2   wert odenen hal
:   else   kimi duwune bilerik . if-in qisa yaziliwidir.
@ if(condition) {
	expr1
} else {
	expr2
}

@if (condition1) {
	expr1
} else if(condition2) {
	expr2
} else {
expr3
}

istediyimiz qeder else if yaza bilerik;

11. What is NaN?
- NaN stands for Not a Number , tipi numberdi .
isNaN(a) methodu ile a tipinin number olub olmadigini yoxlamaq olur
inNaN(string) // true
inNaN(5) // false

12. Explain the meaning of the keyword ‘this’ in JavaScript functions
- this muraciet elediyin objecti qaytarir 
$(‘.test’).click(function(){
	this.text(‘obect referenced’);
})
$(‘.test’) array qaytarir , object arrayi amma click etdikde this hansina kliklemisense onu qaytarir;

13. What is the difference between undefined and not defined in JavaScript?
- 


16. What is functional programming?
- Funksional proqramlasdirmada problemin helli funksiyalara dayanir. Funksiyalarin istifadesi proqramda tekrarlari aradan qaldirir, bu musbet cehetidi. Menfi terefi ise funksiyalar proqramin iwini yavawladir. 

17. What is the difference between classical inheritance and prototypal inheritance?
- classic inheritance class mentiqine dayanir. OOP dillerdeki inhritance mentiqi JS deki inheritance -dan ferqlenir , cunki javascriptde class anlayiwi ferqlidir. javascriptde ierarchic inheritance qurulusu var. Inheritance prototype chain uzre yonelir.

18. What are the pros and cons of functional programming vs object-oriented programming?
# OOP musbet cehetleri:
- her sey object weklinde oldugu ucun asanliq yaradir;
- objectlerin propertileri metodlari oldugu ucun bunlardan istifade kod tekrarinin qarsisini alir;
- modul prinsipi rahat modifikasiya etmeye imkan verir;
- debug daha rahatdi;
# OOP menfi cehetleri:
- daha cox emek teleb edir;
- daha murekkebdi;
- daha cox yaddas tutur;
- her problemin helline uygun deyil;
19. When is classical inheritance an appropriate choice?
- cox nadiren bezi projectlerde istfade olunur.
20. When is prototypal inheritance an appropriate choice?
- ne yalan deyim catmadi valla
21. 


