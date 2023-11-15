# autoPytoEXE
## auto convertation .py files to .exe

.yml files for your repository

every push this program make your .py file to .exe and send to artifacts

For Linux and Windows


RU:
## Авто компилятор питон кода в .ехе файл

Все будет происходить во вкладке actions

Workflow создавать Python Application (можно поэкспериментировать, но я делал с этим)

## Отличия:

### PyInstaller: 
-SFX ехешник (исходный код легко достать)

+Работает отдельно от питона (функции требующие питон не будут работать)

+Время билда 1-5 минут

-Только для виндовс

### Nuitka:
+Код конвертируется в С язык и пакуется в ехе, также его сложнее вскрыть для получения исходников

+Может работать как отдельно от питона, так и с ним (в .yml файле значение у standalone - true/false - без питона/с питоном; 
										в первом случае он создаст только .ехе
										во втором .exe и .cmd, после чего указать путь к питону в цмд файле, и запускать программу через цмд)

-Время билда 2-13 минут (у меня больше 13 небыло)

+Для всех платформ

## Установка:

закинуть файл build.yml в репозиторий/.github/workflows

`ВСЕ СЛОВА ВЫДЕЛЕННЫЕ КАПСОМ ЗАМЕНИТЬ НА СООТВЕСТВУЮЩИЕ ВАШЕМУ АККАУНТУ (юзернейм, репозиторий и тд)`

после чего (если пункты вначале файла были выполнены) у вас при каждом пуше проекта должен начинаться workflow в артефактах которого будут лежать ваши exeшники

никаких токенов не требуется

EN:

## Python code's auto compiler.exe file

Works in conjunction with github

Everything will happen in the actions tab

Workflow create Python App (you can experiment, but I did with this)

## Differences:

### PyInstaller: 
-SFX cache (the source code is easy to get)

+Works separately from python (functions requiring python will not work)

+Build time 1-5 minutes

-Only for windows

### Nuitka:
+The code is converted to C language and packaged in exe, it is also more difficult to open it to get the source code

+Can work both separately from python and with it (in the .yml file, the value of standalone is true/false - without python/with python; 
 in the first case , it will create only .exe
in the second .exe and .cmd, then specify the path to the python in the cmd file, and run the program through the cmd)

-Build time is 2-13 minutes (I didn't have more than 13)

+For all platforms

## Installation:

upload the build file.yml to the repository/.github/workflows

`REPLACE ALL THE WORDS HIGHLIGHTED BY CAPS WITH THE APPROPRIATE ONES FOR YOUR ACCOUNT (username, repository, filename)`

after that (if the items were executed at the beginning of the file), every time you push the project, workflow should start, in the artifacts of which your assistants will lie

no tokens are required
