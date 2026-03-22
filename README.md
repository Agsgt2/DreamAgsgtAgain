# DreamAgsgt
DreamAgsgt is a ~~version of Dreamberd~~ programming language which is owned by the Agsgt Foundation, here are some scripts for the language, also this is fake. Actually.<br>
The text marked with a "*" is a copy or a same script of the DreamBerd language<br>

## If
If is a function which if its input is true, the then output is true, if not, the script excecutes the scripts after the if script, or if it has a `else` counterpart, it runs it <br>
```js
if <score = 5> {
  score = score - 5
}
```

## We
We is a statement randomness, it is complex and may have a table for it, here it is:

|A|B|Out|
|-|-|---|
|F|F|F  |
|F|T|F  |
|T|F|T  |
|T|T|T  |

And i cant froget about the example!
```js
print(We(True, False)) //True
```

## Lifetimes*
Lifetimes are a toggler that makes a duration for scripts, they can be positive by lines or seconds by the example below
```js
print<2l>("I last for 2 lines!") //I last for 2 lines!
print<10s>("I last for 10 seconds!") //I last for 10 seconds!
```
Or they can be negative
```js
print(text) //I may last after my creation...
var text<-1l> = "I may last after my creation..."
```

## Were
Were is a copy of `We`, with the difference that it is more advanced than We and has more inputs and outputs.

|A|B|C|Out|Qwery|
|-|-|-|---|-----|
|F|F|F|F  |F>T  |
|T|F|F|F  |F>T  |
|T|T|F|?  |F=T  |
|F|T|F|F  |F>T  |
|T|F|T|?  |F=T  |
|F|T|T|?  |F=T  |
|F|F|T|F  |F>T  |
|T|T|T|T  |F<T  |

```js
print(Were(T,T,T)) //[True, Qwery: False < True]
```

## Function*
Makes a function with every letter of the word function (only if they are in order)
```js
function add(a,b) {return a + b}
funti sub(a,b) {return a - b}
i mult(a,b) {return a * b}
funi div(a,b) {return a / b}
```
### Async Functions
Same with function, it does not matter the letters, the order is what matters.
```js
async function f0(){ ... }
a f f1(){ ... }
anc fnc f2(){ ... }
```

## Rich text*
More complex text, used for links and stuff
<pre>
  print("<b>Wow!</b>") //<b>Wow!</b>
</pre>

## HTJS*
HTJS is a script that turns from JavaScript into HTML
```js
HTJS.run{
  <h1>HTJS script</h1>
}
```
It has a lot of variants:
```js
print(HTJS.htmltotext(
  <h2>What am i doing here?!?</h2>
)) //What am i doing here?!?

HTJS.functionHTJS <hn "size"=1-6> {
  <HTJS.headersize (size)>
}
```
### New for 2026!
You are free to freely use the `for` argument since DreamAgsgt uses `four`, not `for`.
```js
HTJS.run{
  <label for="hello">Hello!</label>
}
```
And you must ALWAYS use the `HTJSClass` argument instead of the `class` argument.
```js
HTJS.run{
  <h1 HTJSClass="hello">Hello!</h1>
}
```

## Youtube
Uses Youtube search query to play on a window
```js
Youtube.play(Youtube.search("Reaction Reaction"))
```
### Youtube: Extras
You can even use Youtube search query to search in your browser!
```js
let searchYT = Youtube.search("@ATFLURE")
Browser.search(searchYT)
```
### Youtube: New for 2026!
You can now search videos by creator!
```js
let searchYT = Youtube.search("", "@ATFLURE")
```

## DreamlyBerd*
An giant extension with most of DreamBerd commmands!<br>
Import:
```js
from "DreamlyBerd" import * as DreamlyBerd
```
Note: it has a premium version and you can buy it like this:
```js
DreamlyBerd.PremiumBuy()
```
it enables all of the DreamBerd commands!

## Loops
Unlike DreamBerd, DreamAgsgt has various loops.
### For
To create an For loop, you must use `four`
```js
four (let i = 0; i <= 10; 1++){
  print(i)
}
```
You can also create an `four (... of ...)` loop
```js
four (let i of [1, 2, 3, 4]){
  print(i)
}
```
### While
To create an While loop, you must use `wail`
```js
wail(score > 5){
  score++
}
```
You can also do an `do { ... } wail` loop
```js
do {
  score = 5
} wail (score > 5)
```
## Databases
Now we have databases on the cloud!
```js
// @filename: index1.da
database.add("name", "value")

// @filename: index2.da
print(database.get("name")) // value
```
You could also fetch some value when a name gets added
```js
print(database.fetch("name"))
```
You can remove or replace values on the database
```js
database.replace("name", new Date())

database.remove("name")
```
You can also define your own public database!
```js
let database1 = new DataBase("publichost:2763")
database1.add("name")
```
WARNING: You can also add readonly values, just, use them for experimental purpouses.
```js
database.add("pi", 3.14159, true)
```
## Angel3D
You can create an new 3D game instance using
```js
let new3D = new Angel3D()
```
Add an object using
```js
new3D.add(Angel3D.type.Object, "20")
```
Make it move by using
```js
new3D.obj("20").move(20, 50)
```
There are too many functions ._.
## Types
DreamAgsgt also uses types like in TypeScript. The default is any.
```ts
i sum(a: number, b){return a+b}
```
### all
In TypeScript, you can choose `any` or `unknown` for an type which is something else, 
but in DreamAgsgt, we have the `all` type, which is like `any`, but does not disable type 
checking.
```ts
func doSomething(a: all){
  // Do something...
}

// All OK
doSomething(25)
doSomething(new Date())
doSomething({})
```
### none
Instead of using the `undefined` or `null` types for useless inputs, you can use the `none` type!
```ts
func doSomething(a: none){
  // Can't do anything with a, so i won't
}

// OK
doSomething()

doSomething("Hello, World!") // Error: Type "string" is not assignable to type "none"
```
### Automatic `Promise<>` Type
You now don't need to use the annoying `Promise<>` type anymore! Just type an async function
with an return type and you are done!
```ts
asy func fetchSomething(): number { ... } // OK
```
## Booleans
There is now `false`, `disapproved`, `neutral`, `approved`, and `true`.
```js
const a = approved
```
You can now use `==`, `===`, `>`, or `<` to see if an boolean is equal, higher, or lower than
another boolean!
```js
if (true > approved){
  console.log("Hello, World!")
}
```
## Equals*
Did i forget there are 4 types of equal?
### Slightly Equal/`=`
The slightly equal does not matter if an number has the same decimal places or not.
```js
3.141 = 3 // true
```
### Equal/`==`
This checks if an number has atleast 2 decimal numbers equal.
```js
3.141 == 3.142 // true
```
### Strictly Equal/`===`
This checks if all of the decimal numbers are equal.
```js
111.111 === 111.1111 // false
```
### Actually Equal/`====`/`is`
This checks if all of the decimal numbers AND the memory spot are equal.
```js
const pi = 3.141
pi ==== pi // true
3.141 is 3.141 // true
3.142 is 3.141 // false
pi ==== 3.141 // false
```
