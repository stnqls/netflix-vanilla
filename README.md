# ð½ NETFLIX ííì´ì§ ë°ë¼ ë§ë¤ì´ ë³´ê¸°

## ìì±í ííì´ì§ ëª¨ìµ
<img width="80%" src = "https://user-images.githubusercontent.com/81519415/121842564-91de2d00-cd1b-11eb-9dfd-f203b65ffc2e.png"/>
---

### tvì´ë¯¸ì§ì ëìì ì½ìíê¸°
```css
.tv .content-tv {
  position: relative;
}
.tv .content-tv .image-tv {
  position: relative;
  z-index: 2;
}
.tv .content-tv .image-tv img {
  width: 530px;
  height: 398px;
}
.tv .content-tv .tv-video {
  width: 387px;
  height: 216px;
  position: absolute;
  top:80px;
  left: 68px;
}
```
<br/>

### ìì£¼ ë¬»ë ì§ë¬¸ ë²í¼í¨ê³¼ ë§ë¤ê¸°
```css
.QA .qa-list .text {
  width: 815px;
  padding: 31.2px;
  box-sizing: border-box;
  font-size: 26px;
  background-color: #303030;
  display: none;
}
.qa-list .text.open {
  display: block;
}
```
```js
let textArray = document.querySelectorAll('.qa-list .text');
let btnArray = document.querySelectorAll('.qa-list button');
document.querySelectorAll('.qa-list button').forEach(function (i) {
  i.addEventListener('click', function(e){
    const clickedBtnIndex = [...btnArray].indexOf(e.target);
    textArray[clickedBtnIndex].classList.toggle('open');
  })
});
```
