### Cross-cutting 

* Вид функциональности, который встречается на всех уровнях приложения
* Примеры:
	* Логгирование
	* Авторизация
	* Exception Handling
	* Транзакция
	* Кэширование
	* Benchmarking
---
### AOP

#### AOP - Аспекто-ориентрованное программирование, это расширение ООП

* Аспект - cross-cutting аспект программы
* AspectJ - библиотека для написания аспектов
* Spring AOP - базовая функциональность Spring для AOP, использующая AspectJ

![[Pasted image 20230108182944.png]]

---
### Proxy

* Proxy - это обёртки над классами

![[Pasted image 20230108183837.png]]

* JDK proxy умеет оборачивать только публичные методы, а Cglib умеет оборачивать ещё и protected

![[Pasted image 20230108184414.png]]

* Weaving - связывание аспектов с другими объектами кода

* Join point - точка вызова метода
* Pointcut - регулярное выражение для join point
* Advice - функциональность, которая исполняется. В аспекте может быть несколько advices
---
### @EnableAspectJAutoprox

* Подключение Spring AOP функциональности
---
### Чтобы заработало...

1) MVN-dependency aspectj
2) Написать аспект
3) @EnableAspectJAutoproxy на классе конфигурации

---
### Advice

* Advice - действия, которые выполняются помимо Joinpoint
* В аспекте может быть много advice
* Аспекты можно упорядочивать, advice нельзя


Виды Advice:
1) @Before - выполняются перед точкой входа
2) @After - выполняются после точки входа
3) @Around - выполняются до и после
4) @AfterRunning - после того как точка входа выполнилась корректно
5) @AfterThrowing - в случае исключения

![[Pasted image 20230108192347.png]]

![[Pasted image 20230108192358.png]]

![[Pasted image 20230108192408.png]]

![[Pasted image 20230108192417.png]]
![[Pasted image 20230108192425.png]]

---
### Pointcut

Pointcut - язык описания мест Join point

![[Pasted image 20230108202934.png]]
![[Pasted image 20230108203110.png]]
![[Pasted image 20230108203345.png]]

---
### Сравнение Spring AOP и AspectJ

![[Pasted image 20230108205434.png]]
