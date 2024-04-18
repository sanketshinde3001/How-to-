# How to add Custom Fonts in Next-Js

### 1) Add following code in layout.js file
```js
import { Nunito } from "next/font/google"; // Here add font name in bracket
// ....... other imports

const nunito = Nunito({ 
  subsets: ["latin"],
  weight: ['200','300','400','500','600','700','800','900','1000'], // these value changes as per fonts
  variable:'--font-nunito' 
});

// for other fonts , just change the 'nunito' with other name..
```

### 2) Add following code in global.css file
```css
.nunito{
  font-family: var(--font-nunito);
}
```
### 3) Add following code to use font in any file
```js
<p className='nunito'>Be Happyl</p>
```
