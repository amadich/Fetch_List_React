# Fetch_List_React
On this page we specify a name from the array and display an element as an image 🍂
###
You Need First Import Your API :
```js
import Apidata from './db/data.json';
```
Add your Stated , create Function for Collecting your data :
```js
const myap  = Apidata.characters;

  let [ch,setCh] = useState("");
  let [imgname , setImgname] = useState("");

  const show = (id) => {
    let newId = document.getElementsByTagName("select")[0].selectedIndex;
    for(let i = 0 ; i <= 8 ; i++) {
      if (newId === myap[i].id) {
          setCh(myap[i].sprite);
          setImgname(myap[i].slug);
      }
    }
  }
  // ... App function => in Git Files 🍃
```

![image](https://user-images.githubusercontent.com/74735976/215351662-fc17f785-34b1-4b60-8c22-5ddc745d30e3.png)
###
