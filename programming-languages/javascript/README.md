JavaScript Հուշաթերթիկ
--------------------

# For loops

Jacascript-ում և այլ ծրագրավորման լեզուներում գոյություն ունեն ցիկլեր, որոնք հեշտացնում են կատարվելիք աշխատանքը: Ցիկլը հնարավորություն է տալիս կատարել որևէ գործողություն որոշակի քանակությամբ: Նմանօրինակ ցիկլ է **For Loop**-ը Javasript-ում: Այն ստեղծում է հանգույց բաղկացած 3 արտահայտություններից.  
1. փոփոխականի սկզբնական արժեքը    
2. փոփոխականի արժեքների տիրույթը  
3. գործողություն փոփոխականի հետ, որի արդյունքում փոփոխականը ստանում է նոր արժեք, այդ արժեքն էլ ընդունում է փոփոխականը հաջորդ անգամ ցիկլի միջով անցնելիս:  
Ենթադրենք ցանկանում ենք 1-50 թվերը հերթով տպել console-ում:
Առանց for loop-ի կոդը կունենա այս տեսքը ՝
	console.log(1);
	consloe.log(2);
և այսպես 50 անգամ, կօգտագործենք for ցիկլը՝
```javascript
let number = 0;
for(i = 0; i < 50; i++){
   number ++
   console.log(i);
};
``` 	
Տրված օրինակում սահմանում ենք փոփոխական number, այնուհետև սահմանում ենք ցիկլը i-ի սկզբնական արժեքը 0 է, արժեքների տիրույթը մինչև 50ը և գործողությունը փոփոխականի հետ(i++, որը նույնն է ինչ i+1) ստացված արժեքն էլ ամեն անգամ օգտագործվելու է հաջորդ ցիկլի ընթացքում։ Շղթայի հիմնական գործողությունն է տպել console-ում iի արժեքը: Երբ աշխատեցնենք այս կոդը console-ում կտպվեն 1-50 թվերը հերթականությամբ։ 

# While 

```javascript
var i = 0 
while (i <= 10) {
var result = i*2; 
console.log(i+" times 2 is equal "+result); 
i++ ; 
}


```
**While loop**-ը ստեղծում է հանգույց, որը կրկնվում է քանի դեռ փոփոխականի արժեքը համապատասխանում է սահմանված պայմանին։  
Տրված օրինակում ստեղծում ենք փոփոխական i, որի սկզբնական արժեքը 0 է,այնուհետև սահմանում ենք պայմանը(քանի դեռ i-ը փոքր է կամ հավասար 10-ի), սրան հետևում է գործողությունը որը մենք ցանկանում ենք կատարել, ստեղծում ենք մեկ այլ փոփոխական result, որը հավասար է ix2, և տպում ենք console-ում «iը բազմապատկած 2ով հավասար է result», հանգույցի ավարտից հետո iը ընդունում է i+1 արժեքը։ 


# Do/While Loop

```javascript
var i = 0; 
do {
var half = i/2 ; 
console.log("the half of "+i+ " is "+half); 
i++

} while (i<10)

```
**Do While loop**-ը անում է գրեթե նույն բանը ինչ While loop-ը մի պարզ տարբերությամբ, որ Do While Loop-ի մեջ սկզբում սահմանում ենք գործողությունը որը ցանկանում ենք կատարել այնուհետև պայմանը որին պետք է մեր փոփոխականը բավարարի, սա նշանակում է գործողությունը կկատարվի առնվազն մեկ անգամ անկախ նրանից արդյոք մեր փոփոխականի արժեքը համապատասխանում է սահմանված արժեքին թե ոչ:  
Տրված օրինակում ստեղծում ենք փոփոխական i, որի սկզբնական արժեքը 0 է, գործողությունը որը ցանկանում ենք կատարել հետևյալն է ՝ ստեղծել մեկ այլ half փոփոոխական, որը հավասար է iի արժեքը բաժանած 2ի, տպել consoleում «iի կեսը հավասար է half» և կրկնել այս գործողությունը քանի դեռ iը փոքր է կամ հավասար 10ի։ 

# JavaScript Comparison Operators

``` javascript 

```
|  Operators  | Explanation |
| ------------- | ------------- |
| =    | հավասար է արժեքը.  |
| ===   | հավասար է և արժեքը, և տեսակը.  |
| !=   | արժեքը հավասար չէ.  |
| !==  | կամ արժեքը կամ տեսակը հավասար չեն.  |
| >    |  մեծ է. |
| <    | փոքր է.   |
| >=    | մեծ է կամ հավասար. |
| <=  |  փոքր է կամ հավասար.  |
| ?  | պայմանական օպերատոր։ Օգտագործվում է, երբ կա պայման և այդ պայմանին բավարարող երկու հնարավոր արժեք։ Օրինակ. var status = (age >= 18) ? 'adult' : 'minor'; status փոփոխականը կստանա 'adult' արժեքը եթե տարիքը մեծ կամ հավասր է 18ի, այլապես այն ընդունում է ՛minor' արժեքը.  |

---
# JavaScript Functions

There are many ways to define and call functions in JavaScript. Let's review them.

1. Simplest way of defining a Function
```javascript
function speaker() {
    console.log('Hello Wrold!');
}

speaker();
```
Here we define a function `speaker()` and then call it.

2. Assigning Function to a variable. In JavaScript Functions have data so we can assign them to a variable. Here is one way to do it:
```javascript
const speak_again_var = function speak_again_func(){
    console.log('Hello again');
}
speak_again_var();
```
Here we give our function a name - `speak_again_func()` and assign it to a variable named `speak_again_var`. We call our function using *variable* name. If we try to call using function name `speak_again_func()` we will see that it is undefined.

3. Anonymous Functions. As we saw previously giving a name to a function is not very useful, so we can omit it, like this:
```javascript
const speak_again_var2 = function (){
    console.log('Hello again Two');
}
speak_again_var2();
```
This is called an anonymous function.

4. Lambdas.
```javascript
const new_cool_f = (a, b) => {
    return a + b;
}
console.log(new_cool_f(4, 5));
```
Here we omit the word `function` and use parentheses within which we indicate that our function takes two arguments. This style is called Lambda Function.

