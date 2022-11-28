## se41.github.io

#### project devoted to learn GitHub pages by se41 group
#### Current tasks:
- [x] #1 - add main page
- [ ] #2 - add additional pages


## Інструкція із додання сторінок студенів
1. ## Додання самої сторінки
створити сторінку st[далі довільна послідовність символів].markdown із даними розмістити в каталозі https://github.com/TNTU-121-Software-Engineering/se41.github.io/tree/GitHub_Pages/docs/pages

![image](https://user-images.githubusercontent.com/65286819/204229051-943dd6c9-df6b-4b6c-aa23-b951cc43fa08.png)


приклади сторінок: [st1.markdown](https://github.com/TNTU-121-Software-Engineering/se41.github.io/blob/GitHub_Pages/docs/pages/st1.markdown) , [st2.markdown](https://github.com/TNTU-121-Software-Engineering/se41.github.io/blob/GitHub_Pages/docs/pages/st2.markdown) , [st4.markdown](https://github.com/TNTU-121-Software-Engineering/se41.github.io/blob/GitHub_Pages/docs/pages/st4.markdown) 

додати в заголовку посилання на layout: default (якщо не створюється інша розмітка) наступним чином:
```
---
layout: default
---
```

далі розмістити текст та зображення в одному із форматів:
  + форматі markdown, як у прикладах [st2.markdown](https://github.com/TNTU-121-Software-Engineering/se41.github.io/blob/GitHub_Pages/docs/pages/st2.markdown) та [st4.markdown](https://github.com/TNTU-121-Software-Engineering/se41.github.io/blob/GitHub_Pages/docs/pages/st4.markdown)
  + додати код html як у прикладі [st1.markdown](https://github.com/TNTU-121-Software-Engineering/se41.github.io/blob/GitHub_Pages/docs/pages/st1.markdown) //зображення та інші ресурси (js, css) можна розмістити у директорії pages/assets/
 
![image](https://user-images.githubusercontent.com/65286819/204229934-24d031c8-7179-4e99-be83-880a1f76d626.png)

2. ## Додання посилання на сторінку в [index.html ](https://github.com/TNTU-121-Software-Engineering/se41.github.io/blob/GitHub_Pages/docs/_includes/index.html)
  
 ### в файлі додається фрагмент розмітки у список інших де вказується:
```
<a href="{{page.st}} 
```
на st[як було названо в попередньому пункті]

```
<img src="assets/images/" 
<img class="card__thumb" src="assets/images/"
```
на зображення картки і аватарки для неї, які треба додати в папку: https://github.com/TNTU-121-Software-Engineering/se41.github.io/tree/GitHub_Pages/docs/assets/images
```
<h3 class="card__title"> Ім'я Прізвище студента  </h3> 
```
заголовок картки ( Ім'я Прізвище студента) 
```
<span class="card__status">student of group SE-</span> 
``` 
дані про студента
```
<p class="card__description">Description</p>
```
креативний чи не дуже опис картки/сторінки тощо.

### Код який треба змінити:

 ``` 
  <li>
          <a href="{{page.st}}" class="card">
            <img src="assets/images/" class="card__image" alt="" />
            <div class="card__overlay">
              <div class="card__header">
                <svg class="card__arc" xmlns="http://www.w3.org/2000/svg"><path /></svg>                     
                <img class="card__thumb" src="assets/images/img5.png" alt="" />
                <div class="card__header-text">
                  <h3 class="card__title">pig_jacuzzi</h3>
                  <span class="card__tagline"> </span>            
                  <span class="card__status">boss</span>
                </div>
              </div>
              <p class="card__description">Description</p>
            </div>
          </a>
        </li> 
 ```
 
3. ## Останнє  (редагуємо файл index.markdown i about.markdown):

Додаємо в файл [index.markdown](https://github.com/TNTU-121-Software-Engineering/se41.github.io/blob/GitHub_Pages/docs/index.markdown) назву своєї сторінки st[] після link:
i "pages/st[].html" як там вже є

 ![image](https://user-images.githubusercontent.com/65286819/204227106-01c4c1c6-a56f-4e90-81b2-94633f7dffb8.png)


В файлі [about.markdown](https://github.com/TNTU-121-Software-Engineering/se41.github.io/blob/GitHub_Pages/docs/about.markdown) дописуємо своє ймення і посилання на сторінки:

![image](https://user-images.githubusercontent.com/65286819/204227844-b673dca5-b5b8-4749-ad44-724998f623bb.png)




