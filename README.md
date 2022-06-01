# JSON
GIT Homework 1
Все шаги сценария выполняйте в терминале GitBush, Terminal, в папке под гитом.

 1. Создать внешний репозиторий c названием JSON.
 
 		В веб интерфейсе github: create new repository JSON --public

2. Клонировать репозиторий JSON на локальный компьютер.
 
 		$ git clone git@github.com:mariiaAks/JSON.git
		
  3. Внутри локального JSON создать файл “new.json”.
 
	$ cd JSON
	$ touch new.json
		
  4. Добавить файл под гит.
 
	$ git add new.json
 
 5. Закоммитить файл.
 
 		$ git commit -m "Add new file new.json"
		
  6. Отправить файл на внешний GitHub репозиторий.

	$ git push 
		
  7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.
 
	$ vim new.json

	INSERT (кнопка i)
  
 	{
    		"personalInfo": {
    			"firstName": "Мария",
				"middleName": "Романовна",
				"lastName": "Щербатова",
				"amountPets": 0,
				"futureSalary": 100000}
	 }
 	Esc :wq
		
  8. Отправить изменения на внешний репозиторий.

	$ git add new.json
	$ git commit -m "Change file new.json: add personalInfo"
	$ git push
 
 9. Создать файл preferences.json
  
 		$ touch preferences.json
 
 10. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.
 
 	$ vim preferences.json
  	INSERT (кнопка i)
	
	{
    	"favoriteMovie": "Летят журавли",
		"favoriteTVSeries": "Склифосовский",
		"favoriteFood": "Солянка",
		"favoriteSeason": "Лето",
		"travelCountry": "Дания"
	 }
 	Esc :wq 
 
 11. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
 
 	$ cat > sklls.json
 	 {
		"theory": "что такое тестирование, багрепорты, документация, виды, методы, направления тестирования",
		"architecture": "клиент-серверная архитектура, структура http запросов и ответов",
		"API testing": "Тестирование API через Postman",
		"web testing": "DevTools браузеров, снифинг web трафика через Charles и Fiddler",
		"mobile testing": "Android studio, перехват мобильного через Charles и Fiddler",
		"database": "Установка и настройка БД Postgres, основы SQL"
 	} 
 12. Отправить сразу 2 файла на внешний репозиторий.
 
 	$ git add preferences.json sklls.json
  	$ git commit -m "Add 2 files preferences.json sklls.json"
  	$ git push

 13. На веб интерфейсе создать файл bug_report.json.
 
 	Add file - Create new file - Commit new file
 
 14. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 
 	Commit changes
 
 15. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
 
 	Edit file bug_report.json
 
 	{
		"bug_id": 1,
		"title": "Dash line not visible on widget",
		"severity": "major",
		"priority": "high",
		"summary": "",
		"precondition": "Clear screen",
		"stepToReproduce": "1) Add several widgets, 2) Change size some widgets",
		"environment": "1) Redmi Note 7 MIUI 12.5.1.0 android 10 QKQ1.190910.002, 2) Honor 20 pro (YAL-L41), Android 10",
		"expectedResult": "Widgets have a dotted line on all 4 sides",
		"actualResult": "Widgets don't have dotted lines",
		"attachments": ""
	} 

 16. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 
 	Commit changes
 
 17. Синхронизировать внешний и локальный репозиторий JSON
 
 	$ git pull
