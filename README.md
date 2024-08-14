# Angular-Practice
A compilation of Angular coding practices for the MEAN Stack (3.25 batch).

## Angular Testing (May 03)
https://github.com/cocodingnut/angular-testing

## Login Event (May 29)
https://stackblitz.com/edit/angular-csa5bm?file=src%2Fapp%2Fapp.component.ts

## Album Search (Jun 17)
https://github.com/cocodingnut/album_search
https://stackblitz.com/edit/angular-yz7bq6?file=src%2Fapp%2Fapp.component.ts

## Mirack OA*2 (Jun 15)
https://docs.google.com/document/d/1znQZcYZlC3GTjCGMLVOsXY17WwVqqmiLuGUw1A97Scc/edit#heading=h.ut9i8iaah82z
### Login And Registration
https://github.com/cocodingnut/login_and_registration

### User Profile Search
https://github.com/cocodingnut/user_profile_search

## Auto Complete City Name (Jun 24)
https://stackblitz.com/edit/angular-txqexp?file=src%2Fapp%2Fapp.component.ts

## OA*2 (Jun 27)
### Display Star Ratings
https://stackblitz.com/edit/angular-si85qq?file=src%2Fapp%2Fapp.component.ts
  <!-- 十进制Unicode编码 -->
  <p>Decimal Code: &amp;#9733; &#9733;</p>
  <!-- 十六进制Unicode编码 -->
  <p>Hexadecimal Code: &amp;#x2605; &#x2605;</p>
  <!-- 命名字符实体 -->
  <p>Named Entity: &amp;starf; &starf;</p>

### Auto Complete Google Search
https://github.com/cocodingnut/AutoComplete

## UAL Vendor OA (Jul 01) 
https://stackblitz.com/edit/stackblitz-starters-gzdqw9?file=package.json

## Hacker News Jobs Board (Jul 01) 
https://stackblitz.com/edit/stackblitz-starters-jxc6vh?file=package.json

Description: Build a job board that displays the latest job postings fetched from the Hacker News API, with each posting displaying the job title, poster, and date posted.

## Post and Comment (Jul 02) David Live Coding
https://stackblitz.com/edit/stackblitz-starters-gjfqsx?file=package.json

## Colorful Cards (Jul 08) 
https://stackblitz.com/edit/stackblitz-starters-etptgp?file=package.json

## Infinite Scroll (Jul 15)
https://github.com/cocodingnut/InfiniteScroll

## Change Detection from Finra Interview (May 29, Jul 17)
https://stackblitz.com/edit/angular-ivy-ikrznp?file=src%2Fapp%2Fhello.component.ts
https://stackblitz.com/edit/angular-wx49s6?file=src%2Fapp%2Fhello.component.ts,src%2Fapp%2Fapp.component.html,src%2Fapp%2Fapp.component.ts,src%2Findex.html

## Flip Cards (Jul 22)
https://stackblitz.com/edit/stackblitz-starters-vaekqp?file=package.json

## Other Practice:
### Behavior Subject
https://stackblitz.com/edit/angular-q3ywqs?file=src%2Fapp%2Fapp.component.ts

### Custom Attribute Directive
https://stackblitz.com/edit/angular-15-starter-pack-vmtsth?file=src%2Fapp%2Fapp.component.ts

### @Output and Event Emitter
https://stackblitz.com/edit/stackblitz-starters-ng2sj5?file=package.json

### Cards Widget
https://stackblitz.com/edit/stackblitz-starters-adgfw3?file=src%2Fmain.ts

### Template Driven Form
https://stackblitz.com/edit/angular-ssdwkz?file=src%2Fapp%2Fapp.component.ts

### Todo List
### Calculator
### Calendar
https://stackblitz.com/edit/stackblitz-starters-dhxsat?file=src%2Fapp%2Fcalendar%2Fcalendar.component.css


### Reactive Form
### Custom Pipe and Directive

## Tips and Resources:
### Angular Offcial Document
https://angular.dev/

Angular 17 Grammer
```typescript
 template: `<ul>
            @for (address of addresses; track address){
               <li>
                <app-address [address]='address'></app-address>
               </li>
            }
             </ul>`

  template: `<ul>
               <li *ngFor="let address of addresses">
                <app-address [address]='address'></app-address>
               </li>
             </ul>`
```

*ngFor="let item of upArray; let i = index" 
@for (item of upArray; track item;  let i = $index){}

```typescript
@if (){
}
@else {
}
```

## Angular’s main libraries, versions, and functionalities:
import { CommonModule } from '@angular/common'; 
What CommonModule Includes:
	1.	Common Directives:
	•	NgIf: Conditionally includes or excludes a template based on the value of an expression.
	•	NgForOf: Iterates over a collection (like an array) and repeats a template for each item.
	•	NgSwitch, NgSwitchCase, NgSwitchDefault: Allows for conditional rendering of templates based on the value of an expression.
	•	NgClass, NgStyle: Dynamically adds or removes CSS classes and styles based on expressions.
	2.	Common Pipes:
	•	DatePipe: Formats dates according to a given format.
	•	UpperCasePipe, LowerCasePipe: Transforms text to uppercase or lowercase.
	•	CurrencyPipe: Formats numbers as currency.
	•	JsonPipe: Converts objects to JSON strings.
	•	DecimalPipe: Formats numbers with decimal points.
	•	PercentPipe: Formats numbers as percentages.
	3.	Common Services:
	•	Location: Provides access to the browser’s URL and allows for navigation.
	•	Title: Allows setting the title of the current HTML document.

 
Array:
`Array.from()` 是一个 JavaScript 内置方法，用于从类数组对象或可迭代对象（如 `Map`、`Set`、字符串）创建一个新的数组实例。这个方法非常灵活，也可以用于数组的浅拷贝、将对象转化为数组，以及通过映射函数创建特定模式的数组。

### 语法

```javascript
Array.from(arrayLike [, mapFn [, thisArg]])
```

### 参数

1. **`arrayLike`**: 必需。类数组对象或可迭代对象，例如 `arguments` 对象、`NodeList`、`Set`、`Map` 等。
  
2. **`mapFn`**: 可选。一个映射函数，用于在新数组创建时对每个元素进行处理（类似于 `Array.prototype.map`）。这个函数会接收两个参数：
   - 当前元素的值
   - 当前元素的索引

3. **`thisArg`**: 可选。执行 `mapFn` 函数时 `this` 的值。

### 示例用法

1. **从类数组对象创建数组**:

```javascript
let arrayLike = { length: 3, 0: 'a', 1: 'b', 2: 'c' };
let arr = Array.from(arrayLike);

console.log(arr); // ['a', 'b', 'c']
```

2. **从字符串创建数组**:

```javascript
let str = 'hello';
let arr = Array.from(str);

console.log(arr); // ['h', 'e', 'l', 'l', 'o']
```

3. **从 Set 创建数组**:

```javascript
let set = new Set(['a', 'b', 'c']);
let arr = Array.from(set);

console.log(arr); // ['a', 'b', 'c']
```

4. **使用映射函数创建数组**:

```javascript
let arr = Array.from([1, 2, 3], x => x * 2);

console.log(arr); // [2, 4, 6]
```

5. **创建指定长度的数组**:

```javascript
let arr = Array.from({ length: 5 }, (_, i) => i + 1);

console.log(arr); // [1, 2, 3, 4, 5]
```

### 应用场景

- **将类数组对象转化为数组**: 可以将 `arguments` 对象或 `NodeList` 转化为真正的数组，方便使用数组的各种方法。
  
- **浅拷贝数组**: 使用 `Array.from(array)` 可以创建一个浅拷贝的数组。

- **数组填充**: 使用 `Array.from` 结合映射函数，可以生成特定规则的数组（如范围、模式等）。

### 总结

`Array.from()` 是一个强大的工具，允许从各种类数组或可迭代对象中创建数组，并提供了在创建过程中对元素进行处理的能力。它的应用场景广泛，能够有效地解决许多数组操作的问题。
