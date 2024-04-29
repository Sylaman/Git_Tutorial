# Основы Git

Git — самая популярная в мире распределённая система контроля версий. Линус Торвальдс, разработчик ядра ОС Linux, создал этот инструмент ещё в 2005 году, а сегодня Git активно поддерживается как проект с открытым исходным кодом. Огромное количество открытых и коммерческих проектов используют Git для контроля версий.

В данной статье перечисляются самые основные команды, которые следует знать разработчику, чтобы освоить управление репозиториями GitHub на высоком уровне. Ознакомиться с ними будет полезно как новичкам, так и опытным разработчикам.

### 30 основных команд, которые сделают из вас мастера Git 

**1. Как задать имя пользователя и адрес электронной почты**  

Имя пользователя нужно, чтобы привязывать коммиты к вашему имени. Это не то же самое, что имя пользователя учётной записи GitHub, с помощью которого выполняется вход в профиль на GitHub. Задать или изменить имя пользователя можно с помощью команды git config. Новое имя будет автоматически отображаться в последующих коммитах, отправленных на GitHub через командную строку. Если хотите скрыть своё реальное имя, можно использовать в качестве имени пользователя Git произвольный набор символов.
```
git config --global user.name "Tara Routray"
```  
Кроме того, командой git config можно изменять адрес электронной почты, привязанный к вашим коммитам Git. Новый адрес электронной почты будет автоматически отображаться во всех дальнейших коммитах, поданных на GitHub через командную строку.  
```
git config --global user.email "dev@tararoutray.com"
```  

**2. Кэширование учётных данных**

Кэшировать учётные данные можно с помощью параметра config с флагом --global. Так вы избавитесь от необходимости вручную вводить имя пользователя и пароль при создании нового коммита.  
```
git config --global credential.helper cache
```  

**3. Инициализация репозитория**  

Создать пустой репозиторий Git или вновь инициализировать существующий можно параметром init. При инициализации он создаст скрытую папку. В ней содержатся все объекты и ссылки, которые Git использует и создаёт в истории работы над проектом.  
```
git init
```   

**4. Добавление отдельных файлов или всех файлов в область подготовленных файлов**  

Добавить отдельный файл в область подготовленных файлов можно параметром add с указанием имени файла. Просто замените somefile.js на актуальное имя.  
```
git add somefile.js
```   
Кроме того, можно добавить все файлы и папки в эту область, предоставив wildcard . вместо имени файла:
```
git add .
```   

**5. Проверка статуса репозитория** 

Просмотреть статус нужного репозитория можно по ключевому слову status: его действие распространяется на подготовленные, неподготовленные и неотслеживаемые файлы.  
```
git status
```

### Остальное добавлю позже, пока изучи это!