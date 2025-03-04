## 📌 Работа с DOM в JavaScript

### **1. Получение элементов**
```js
let title = document.getElementById("title"); // По ID
let button = document.querySelector(".btn"); // По селектору
let items = document.querySelectorAll(".item"); // Все элементы по селектору
let querly = document.querySelector('[data-js-slider]');
```
📌 `querySelector()` универсальный метод, а `querySelectorAll()` возвращает **список элементов**.

---

### **2. Изменение содержимого**
```js
title.innerText = "Новый заголовок"; // Только текст
button.innerHTML = "<b>Кликни меня</b>"; // HTML-код внутри
```
📌 `innerText` меняет **только текст**, `innerHTML` изменяет **весь HTML**.

---

### **3. Изменение стилей**
```js
title.style.color = "red";  // Меняет цвет текста
button.style.backgroundColor = "blue";  // Цвет фона
```
📌 Стили можно менять через `style.property`.

---

### **4. Добавление элементов**
```js
let newDiv = document.createElement("div");
newDiv.innerText = "Привет, мир!";
document.body.appendChild(newDiv); // Добавить в конец body
```
📌 `createElement()` создаёт новый HTML-элемент.

---

### **5. Удаление элементов**
```js
newDiv.remove();  // Удаление элемента
```
📌 `remove()` удаляет элемент из DOM.

---

### **6. Обработчики событий**
#### 📌 Клик по кнопке
```js
button.addEventListener("click", () => {
    alert("Вы нажали кнопку!");
});
```
#### 📌 Ввод текста
```js
let input = document.querySelector("#nameInput");
input.addEventListener("input", () => {
    console.log("Вы ввели:", input.value);
});
```
📌 `addEventListener()` добавляет обработчики событий.

---

### **7. Изменение атрибутов**
```js
let link = document.querySelector("a");
link.setAttribute("href", "https://google.com");
console.log(link.getAttribute("href")); // Получить атрибут
```
📌 `setAttribute()` меняет атрибуты, `getAttribute()` получает их.

---

### **8. Работа с классами**
```js
title.classList.add("highlight"); // Добавить класс
button.classList.remove("btn"); // Удалить класс
button.classList.toggle("active"); // Переключить класс
```
📌 `classList` удобен для работы с классами.

---

## 📌 **Вывод**
✅ **`getElementById()` / `querySelector()`** – поиск элементов.  
✅ **`innerText` / `innerHTML`** – изменение содержимого.  
✅ **`style.property`** – изменение стилей.  
✅ **`createElement()` / `appendChild()`** – создание и добавление элементов.  
✅ **`remove()`** – удаление элемента.  
✅ **`addEventListener()`** – обработка событий.  
✅ **`setAttribute()` / `getAttribute()`** – работа с атрибутами.  
✅ **`classList`** – управление классами.  

📌 Теперь у тебя есть шпаргалка по работе с DOM! 🚀

