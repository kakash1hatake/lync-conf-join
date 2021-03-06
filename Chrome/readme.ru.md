# Шаги для Google Chrome

[Русский](./readme.ru.md) | [English](./readme.md)

1. При настройке *regiser_mime.sh* нужно раскомментировать протокол *lync15* или *lync* (в моем случае это был lync15).
2. Копируем *xdg-open* например в *$HOME/bin* и делаем его исполняемым
```
chmod +x $HOME/bin/xdg-open
```
3. Добавляем каталог куда копировали *xdg-open* в PATH в профайле вашего шелла(я использую bash и в моем случае это *$HOME/.bash_profile*)
```
export PATH="$HOME/bin:$PATH"
```
4. Открываем приглашение на митинг из емейл приглашения и в открывшемся окне браузера на вопрос "запустить xdg-open" говорим *да*. Если Pidgin запущен и все прошло хорошо, то появится всплывающее окно конференции.

# Примечания
Файл *xdg-open* взят из моей системы Linux Mint 19.2 Tina. 
Т.к. я использую десктоп Xfce, то я пропатчил только функцию *open_xfce*. Проделаные изменения можно увидеть в истории коммитов на файле.
Если вы хотите добавить поддержку других дистрибутивов или десктопов, то потребуется поменять файл под себя(если ссылки корректно не открываются у вас через xdg-open).

# Contribution
Если вы хотите добавить ваши изменения в основную ветку проекта, заведите тикет\пулреквест с приложеными патчами.
