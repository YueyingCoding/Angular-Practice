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
draw the layout then implement with logic and variables
https://stackblitz.com/edit/stackblitz-starters-dhxsat?file=src%2Fapp%2Fcalendar%2Fcalendar.component.css
event binding:
```
<td (click)="onClick(date)"> {{date!==0? date:''}}</td>
```
end>length时，取length，不会报错
```
array.slice(start, end)
```
border-collapse: Adjacent cells have shared borders (the collapsed-border table rendering model).
```
border-collapse: collapse;
```


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
1. Common Directives: NgIf, NgFor, NgClass, NgStyle
2. Common Pipes: DatePipe, UpperCasePipe, CurrencyPipe, JsonPipe
3. Common Services: Location: Provides access to the browser’s URL and allows for navigation.


```javascript
string.substr(start, length)
string.slice(start, end) - End position (up to, but not including).
//substring does not support negative indexing.
string.substring(start, end) - End position (up to, but not including).
```

