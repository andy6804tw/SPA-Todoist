
## 取得標籤id的文字內容

```js
// 取得 input 內容
document.getElementById('item').value;
// 取得元素內容
document.getElementById('item').innerText;
```

## 元件點擊監聽事件

```js
document.getElementById('add').addEventListener('click',()=> {
});
```

## 動態新增元素

```js
const item=document.createElement('li');
item.innerText=text; //元素內增加文字
item.classList.add('text'); //將此元素新增class="text"
item.innerHTML="<div>...</div>" //元素內塞入子標籤(子child)
```


## 動態渲染

```js
const list=document.getElementById('todo');

// list塞入一筆todo item
// 依序塞入
list.appendChild(item);
// 每次塞入都會為第一筆置頂
list.insertBefore(item,list.childNodes[0]);
```


inspired by: https://www.youtube.com/watch?v=2wCpkOk2uCg
