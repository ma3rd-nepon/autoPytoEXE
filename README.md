# autoPytoEXE
## auto convertation .py files to .exe

.yml files for your repository

every push this program make your .py file to .exe and send to artifacts

For Linux and Windows


RU:
## Авто компилятор питон кода в .ехе файл

В данном репозитории 2 ймл файла: в одном используется PyInstaller, в другом Nuitka

## Отличия:

### PyInstaller: 
-SFX ехешник (исходный код легко достать)

+Работает отдельно от питона (функции требующие питон не будут работать)

+Время билда 1-5 минут

-Только для виндовс

### Nuitka:
+Код конвертируется в С язык и пакуется в ехе, также его сложнее вскрыть для получения исходников

+Может работать как отдельно от питона, так и с ним
(настройки компиляции кода)
![standalone](https://github.com/ma3rd-nepon/autoPytoEXE/blob/main/auto_compiling_to_exe/standalone.png)

-Время билда 2-13 минут (у меня больше 13 небыло)

+Для всех платформ

## Установка:

Все будет происходить во вкладке actions

Workflow создавать Python Application (можно поэкспериментировать, но я делал с этим)

закинуть файл .yml (выберите нужный, 2 сразу вам не понадобятся) в репозиторий/.github/workflows

![ymls](https://github.com/ma3rd-nepon/autoPytoEXE/blob/main/auto_compiling_to_exe/ymls.png)

`ВСЕ СЛОВА ВЫДЕЛЕННЫЕ КАПСОМ ЗАМЕНИТЬ НА СООТВЕСТВУЮЩИЕ ВАШЕМУ АККАУНТУ (юзернейм, репозиторий и тд)`

после чего (если пункты вначале файла были выполнены) у вас при каждом пуше проекта должен начинаться workflow в артефактах которого будут лежать ваши exeшники

![actions](https://github.com/ma3rd-nepon/autoPytoEXE/blob/main/auto_compiling_to_exe/actions.png)

![workflows](https://github.com/ma3rd-nepon/autoPytoEXE/blob/main/auto_compiling_to_exe/workflows.png)

![artifacts](https://github.com/ma3rd-nepon/autoPytoEXE/blob/main/auto_compiling_to_exe/artifacts.png)

никаких токенов не требуется

## Настройка Nuitka для ехешника работающего в связке с питоном

домой приду напишу подробно все

