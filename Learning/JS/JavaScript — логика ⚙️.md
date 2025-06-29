## Что такое JavaScript?

JavaScript (JS) — это **язык программирования**, который позволяет делать сайты живыми, динамичными и интерактивными.  
Когда ты кликаешь на кнопку, вводишь текст в форму, листаешь слайдер, отправляешь данные на сервер — это всё делает JavaScript.

## Что умеет JavaScript?

- Реагировать на действия пользователя (клики, ввод текста, скролл и т.д.)
- Менять содержимое страницы "на лету"
- Выполнять расчёты, проверки, анимации
- Общаться с сервером (отправлять и получать данные без перезагрузки страницы)
- Создавать полноценные приложения в браузере (SPA — Single Page Applications)

# Как подключается JavaScript?

1. Внутри тега `<script>`
```html
<script>
	console.log('Привет, мир!');
</script>
```

2. Внешний файл
```html
<script src="script.js"></script>
```

---

## Основы JavaScript

### 1. Переменные

Места, где мы храним данные.

```javascript
let name = 'Андрей';
const age = 25;
```

- `let` - современный стандарт, можно менять значение.
- `const` - постоянная, нельзя менять.
- `var` - устарело, но встречается.

### 2. Типы данных

- Числа: `let x = 5;`
- Строки: `let name = 'Кот';`
- Булевы: `let isTrue = true;`
- Массивы: `let list = [1,2,3];`
- Объекты: `let user = {name: 'Иван', age: 30}`
- Null/Undefined - пусто или не определено

### 3. Условия

```javascript
if (age > 18) {
	console.log('Ты взрослый');
} else {
	console.log('Ты ещё малой');
}
```

### 4. Циклы

```javascript
for (let i = 0; i < 5; i++) {
	console.log(i);
}
```

### 5. Функции

```javascript
function greet(name) {
	console.log('Привет, ' + name);
}

greet('Имя');
```

### 6. Работа с элементами страницы (DOM)

```javascript
document.querySelector('button').addEventListener('click' () => {
	document.querySelector('h1').textContent = 'Ты нажал на кнопку';
});
```
Это позволяет менять страницу без перезагрузки.

### 7. События

- Клики: `click`
- Наведения: `mouseover`
- Ввод в поле: `input`
- Отправка формы: `submit

```javascript
document.querySelector('input').addEventListener('input' (e) => {
	console.log('Ты ввёл: ' + e.target.value);
});
```

### 8. Массивы и объекты

```javascript
let fruits = ['яблоко', 'банан', 'вишня'];
console.log(fruits[1]); // банан

let user = {name: 'Вася', age: 20};
console.log(user.name); // Вася
```

### 9. Простая анимация

```javascript
document.querySelector('button').addEvetListener('click', () => {
	document.querySelector('h1').style.transform = 'scale(1.2)';
});
```