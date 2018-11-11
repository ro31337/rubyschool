# faq rubyschool

1. Какой Linux дистрибутив использовать?

Ответ: ubuntu-based дистрибутив, например,

- Linux Mint Cinnamon. linux mint 18 sarah cinnamon 64 bit.
  После запуска Live CD необходимо установить Mint из ярлыка на рабочем столе.
- elementary OS
  <a href="https://elementary.io/">A fast and open replacement for Windows and macOS</a>

2. Как определить, какой гем нужен для работы? Гуглить по сайтам? И как конкретно обращаться с подключенным гемом? Ковыряться с документации и смотреть какие функции есть?

Ответ: Ввести в гугле "gem for ... site:github.com"
Когда нашли нужный gem то ввести в гугле:
(если это gem devise например): "devise vs"
и гугл выдаст список результатов

https://www.google.com/#newwindow=1&q=gem+%22devise+vs%22

https://www.google.com/#newwindow=1&q=gem+%22cancancan+vs%22

3. Какие основные команды в linux?  
   Ответ:  
   `pwd` - напечатать текущую директорию  
   `cd bar` - войти в директорию bar  
   `cd ..` - подняться на уровень вверх  
   `cd ~` - войти в домашнюю директорию  
   `mkdir foo` - создать директорию foo  
   `ls` - вывести список файлов  
   `ls -lah` - вывести подробный список  
   `ruby app.rb` - запустить программу app.rb

4. Чем заменить стандартный bash?  
   Ответ:  
   Установить **oh my zsh** вместо стандартного **bash**.  
   Отсюда: https://github.com/robbyrussell/oh-my-zsh#basic-installation

5. Как установить vm-ware-tools?  
   Ответ:
   ```consolecls
   foo@bar:~$ apt-get update
   foo@bar:~$ apt-get upgrade
   foo@bar:~$ reboot
   foo@bar:~$ apt-get install open-vm-tools-desktop
   foo@bar:~$ reboot
   ```
6. По умолчанию в репозиториях операционной системы устаревшая версия git'а
   Как установить актуальную версию (https://youtu.be/f6b5p5ss1nA)
   Ответ:

```console
foo@bar:~$ add-apt-repository ppa:git-core/ppa
foo@bar:~$ apt-get update
foo@bar:~$ apt-get install git
```
