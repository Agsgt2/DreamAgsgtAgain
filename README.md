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

And I can't forget about the example!
```js
print(We(True, False)) //True
```

## Lifetimes*
Lifetimes are a toggler that makes a duration for scripts; they can be positive by lines or seconds, as shown in the example below
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
HTJS is a script that turns JavaScript into HTML
```js
HTJS.run{
  <h1>HTJS script</h1>
}
```
It has a lot of variants:
```js
print(HTJS.htmltotext(
  <h2>What am I doing here?!?</h2>
)) //What am I doing here?!?

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
Uses a YouTube search query to play on a window
```js
Youtube.play(Youtube.search("Reaction Reaction"))
```
### Youtube: Extras
You can even use a YouTube search query to search in your browser!
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
A giant extension with most of DreamBerd commands!<br>
Import:
```js
from "DreamlyBerd" import * as DreamlyBerd
```
Note: it has a premium version, and you can buy it like this:
```js
DreamlyBerd.PremiumBuy()
```
It enables all of the DreamBerd commands!

## Loops
Unlike DreamBerd, DreamAgsgt has various loops.
### For
To create a for loop, you must use `four`
```js
four (let i = 0; i <= 10; 1++){
  print(i)
}
```
You can also create a `four (... of ...)` loop
```js
four (let i of [1, 2, 3, 4]){
  print(i)
}
```
### While
To create a while loop, you must use `wail`
```js
wail(score > 5){
  score++
}
```
You can also do a `do { ... } wail` loop
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
You can remove or replace values in the database
```js
database.replace("name", new Date())

database.remove("name")
```
You can also define your own public database!
```js
let database1 = new DataBase("publichost:2763")
database1.add("name")
```
WARNING: You can also add read-only values and use them for experimental purposes.
```js
database.add("pi", 3.14159, true)
```
### The recently new!
You can now add or read functions to databases!
```js
database.add("add", (a, b)=>a+b)
const add = database.get("add")

add(2, 5) // 7
```
## Angel3D
You can create a new 3D game instance using
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
In TypeScript, you can choose `any` or `unknown` for a type that is something else, 
But in DreamAgsgt, we have the `all` type, which is like `any`, but does not disable type 
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
  // Can't do anything with a, so I won't
}

// OK
doSomething()

doSomething("Hello, World!") // Error: Type "string" is not assignable to type "none"
```
### Automatic `Promise<>` Type
You no longer need to use the annoying `Promise<>` type anymore! Just type an async function
with a return type, and you are done!
```ts
asy func fetchSomething(): number { ... } // OK
```
## Booleans
There is now `false`, `disapproved`, `neutral`, `approved`, and `true`.
```js
const a = approved
```
You can now use `==`, `===`, `>`, or `<` to see if a boolean is equal, higher, or lower than
another boolean!
```js
if (true > approved){
  console.log("Hello, World!")
}
```
## Equals*
Did I forget there are 4 types of equal?
### Slightly Equal/`=`
The slightly equal does not matter if a number has the same decimal places or not.
```js
3.141 = 3 // true
```
### Equal/`==`
This checks if a number has at least 2 decimal numbers equal.
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
## Geometry Dash API
The Geometry Dash API can be imported using
```js
from "gdapi" import * as gdapi
```
You can search levels by name and ID
```js
let level1 = gdapi.search("Trigger Abuse")
let level2 = gdapi.search(136353284n /* For levels after 1.5, we recommend using bigints.*/)
```
This is what the Geometry Dash API returns when searching a level: <br>
|Data Name|Data Type|
|---------|---------|
|name     |string   |
|id       |number/bigint|

You can also play a level if you have the Geometry Dash API Extension for Geometry Dash.
```js
gdapi.play(level1.id) // Opens Geometry Dash with the ID of the level copied.
```
## Variables, Lets, and Consts*
There are various ways that you can define variables.
### Temporary/Constant Constant Variables `const const`/`const ... as const`
To create a temporary variable, you could do
```ts
const const temp1 = 123
const temp2 = 456 as const

temp1 = 789 // Error: Variable "temp1" is a temporary variable
```
### Variable Constant Variables `let const`/`var const`/`let ... as const`/`var ... as const`
Variable Constant Variables are variables that can be edited, but their children can't
```ts
let const vcon1 = 123
let vcon2 = [4, 5, 6] as const

// OK
vcon2 = [7, 8, 9] // Does not need as const

vcon2[1] = 10 // Error: Variable "vcon2" is a variable constant variable
```
### Constant Variable Variables `const let`/`const var`/`const ... as let`/`const .. as var`
Constant Variable Variables are the contrary of Variable Constant Variables. The children can 
get edited, but their parent can't
```ts
const let cvar1 = 123
const cvar2 = [4, 5, 6] as var

// OK
cvar2[1] = 5.5

cvar2 = [7, 8, 9] // Error: Variable "cvar2" is a constant variable variable
```
### Permanent/Constant Constant Constant Variables `const const const`/`const const ... as const`/`const ... as const const`/`const ... as const as const`
These variables affect both your code and the global code, it permanently leaves a mark on everyone's code. Please use this for experimental purposes.
```ts
const const const pi = 3.14159
```
## Owningmentship <!-- TODO: fix this crap cuz why tf not -->
ik this name is balls, but if your clone of this does not have "DreamAgsgtAgain", then it is owned by the DreamAgsgtAgain Corp.
- `MyDreamAgsgtAgain` is NOT owned by the DreamAgsgtAgain Corp.
- `RustPlus` is owned by the DreamAgsgtAgain Corp.
