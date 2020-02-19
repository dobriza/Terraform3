  **Пошаговая инструкция для Windows**
1. [Скачать компилятор go для Windows](https://dl.google.com/go/go1.13.8.windows-amd64.msi)
2. Проверить, что инсталлятор добавил запись в переменную окружения PATH для пользователя
`%USERPROFILE%\go\bin `
3. Проверить, что инсталлятор добавил запись в системную переменную PATH
`C:\Go\bin`
4. Убедится, что в PS теперь доступна команда go 
5. Создать в рабочем каталоге C:\Go\bin папку \src\github\terraform-providers\terraform-provider-vscale
6. Склонировать репо с плагином vscale в каталог terraform-provider-vscale 
7. Для инициализации модуля в каталоге terraform-provider-vscale, выполнить команду
`go mod init`
Вывод будет примерно такой 
`go: creating new go.mod: module github/terraform-providers/terraform-provider-vscale`
`go: copying requirements from Gopkg.lock`
8. Выполнить go build
9. Если ошибок при билде не будет, то в каталоге terraform-provider-vscale появится terraform-provider-vscale.exe