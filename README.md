<h1 >Проект по автоматизации API тестирования сервиса <a href="https://reqres.in/ ">Reqres.in</a></h1>

<p align="center">  
<img src="media/reqres.in.png" alt="MainLogo" width="950"/></a>  
</p>

# 🧾 Содержание:

- [Технологии и инструменты](#технологии-и-инструменты)
- [Реализованные проверки](#Реализованные-проверки)
- [Запуск тестов (Сборка в Jenkins и параметры)](#запуск-тестов-сборка-в-jenkins)
- [Запуск тестов (Из терминала)](#запуск-тестов-из-терминала)
- [Интеграция с Allure Report](#allure-report)
- [Интеграция с Allure TestOps](#интеграция-с-allure-testops)
- [Интеграция с Jira](#интеграция-с-jira)
- [Уведомление в Telegram о результатах выполнения автоматизированных тестов](#уведомление-в-telegram-о-результатах-выполнения-автоматизированных-тестов)

<a id="технологии-и-инструменты"></a>

## 🔨 Технологии и инструменты:
 <a href="https://www.java.com/"><img src="/media/java.svg" width="50" height="50"  alt="Java"/></a>  <a href="https://www.jetbrains.com/idea/"><img src="media/IJ.svg" width="50" height="50"  alt="IDEA"/></a>  <a href="https://github.com/"><img src="media/gitHub.svg" width="50" height="50"  alt="Github"/></a>  <a href="https://junit.org/junit5/"><img src="media/jUnit5.svg" width="50" height="50"  alt="JUnit 5"/></a>  <a href="https://gradle.org/"><img src="media/gradle.svg" width="50" height="50"  alt="Gradle"/></a>  <a href="https://github.com/allure-framework"><img src="media/allure.svg" width="50" height="50"  alt="Allure"/></a>  <a href="https://allure.autotests.cloud/"><img src="media/AllureTestOps.svg" width="50" height="50" alt="Allure_TO" title="Allure_TO"/></a>  <a href="https://www.jenkins.io/"><img src="media/jenkins.svg" width="50" height="50"  alt="Jenkins"/></a>  <a href="https://www.atlassian.com/software/jira/"><img src="media/Jira.svg" width="50" height="50" alt="Jira" title="Jira"/></a>  <a href="https://web.telegram.org/"><img src="media/telegram.svg" width="50" height="50" alt="Telegram"/></a>   <a href="https://rest-assured.io/"><img src="/media/RestAssured.svg" width="50" height="50"  alt="RestAssured"/></a> 

В данном проекте автотесты написаны на **Java**. Для сборки проекта в
среде IntelliJ IDEA используется **Gradle**. **JUnit 5** задействован в качестве фреймворка модульного тестирования, а
**RestAssured** используется для тестирования API.
Запуск тестов выполняется из **Jenkins**, и вся работа по управлению проектом и отслеживанию задач выполняется с
использованием **Jira**. **Allure Report**, **AllureTestOps** и **Telegram Bot** используются для визуализации
результатов тестирования.

<a id="Реализованные-проверки"></a>

## 🏁 Реализованные проверки:

- Успешное создание нового пользователя
- Успешная регистрация пользователя
- Отправка на регистрацию с незаполненными email/password
- Обновление данных пользователя
- Удаление пользователя


<a id="запуск-тестов-сборка-в-jenkins"></a>

## <img alt="Jenkins" height="25" src="media/jenkins.svg" width="25"/> Сборка в [Jenkins](https://jenkins.autotests.cloud/job/API_Diplom_Tests_amtrsv/)

<p align="center">  
<img src="media/jenkins.png" alt="Jenkins" width="950"/></a>  
</p>

<a id="запуск-тестов-из-терминала"></a>

## 🚀 Команда для запуска автотестов из терминала

```bash  
gradle clean test 
```

<a id="allure-report"></a>

## <img alt="Allure" height="25" src="media/allure.svg" width="25"/> </a>Интеграция с <a target="_blank" href="https://jenkins.autotests.cloud/job/API_Diplom_Tests_amtrsv/allure/">Allure Report</a>

- Основная страница отчёта
<p align="center">  
<img title="Allure Overview Dashboard" src="media/allure2.png" width="850">  
</p>  

- Тест-кейсы

<p align="center">  
<img title="Allure Tests" src="media/allure1.png" width="850">   
</p>

## <img alt="Allure_TO" height="25" src="media/AllureTestOps.svg" width="25"/> </a>Интеграция с <a target="_blank" href="https://allure.autotests.cloud">Allure TestOps</a>

- Основная страница отчёта

<p align="center">  
<img title="Allure TestOps Dashboard" src="media/allure5.png" width="850">  
</p>  

- Страница запуска
  
<p align="center">  
<img title="Allure TestOps launch" src="media/allure6.png" width="850">  
</p>

<a id="#интеграция-с-jira"></a>
## <img alt="Jira" height="25" src="media/Jira.svg" width="25"/></a> Интеграция с <a target="_blank" href="https://jira.autotests.cloud/browse/HOMEWORK-1111">Jira</a>

<p align="center">  
<img title="Jira" src="media/jira1.png" width="">  
</p>

____

<a id="уведомление-в-telegram-о-результатах-выполнения-автоматизированных-тестов"></a>

## <img alt="Allure" height="25" src="media/telegram.svg" width="25"/></a> Уведомление в Telegram при помощи бота

____
<p align="center">  
<img title="TG Overview" src="media/telegram.png" width="400">  
</p>

____
