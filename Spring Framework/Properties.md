### Property файлы

* Нужны для конфигурации приложений
* Хранятся в ресурсах
* Могут фильтроваться мавеном
---
### Подключение property файлов

![[Pasted image 20230105174754.png]]

---
### Как использовать?

* Использовать SpEL (Spring Expression Language)
* C помощью плейсхолдера ${name} можно получать свойства из property файлов
* Для использования этого придётся настроить PropertyPlaceholderConfigurer (В SpringBoot он уже есть)
---
### Чтобы плейсхолдеры заработали нужно объявить специальный бин
![[Pasted image 20230105175312.png]]

---
### @Value

* Используется для применений значений в property файлах

![[Pasted image 20230105175558.png]]
![[Pasted image 20230108180953.png]]

---
### Локализация

* Internationalized (i18n) и Localization(l10n)
* Чтобы локализовать приложение нужны Bundle 

![[Pasted image 20230105193230.png]]
![[Pasted image 20230105193218.png]]
![[Pasted image 20230105193243.png]]
![[Pasted image 20230105193345.png]]
