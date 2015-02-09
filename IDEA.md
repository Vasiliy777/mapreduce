### Настройка Intellij IDEA
Можно писать задачи прямо на кластере в Intellij IDEA (или Eclipse, кому как удобно). 

На Ubuntu при подключении по ssh нужно подключаться так:
$ ssh <LOGUN>@bds01.vdi.mipt.ru -X -C
(скорее всего при первом подключении с -X будет написано, что не удалось - переподключитесь).

IDEA уже есть на сервере тут: /usr/local/idea-IC-139.225.3
Можно сделать символьлую ссылку в удобную для себя директорию (на сервере):
$ ls -s /usr/local/idea-IC-139.225.3 ~/IDEA
После этого можно запускать IDEA так:
$ ~/IDEA/bin/idea.sh
при этом окошко будет пробрасываться вам, хотя IDEA будет работать на удаленной машине. 
То есть, запуская с -X вы говорите, что окошки надо отображать у вас на дисплее, а -C отвечает за сжатие (можно и без него).

Если у вас Windows, то скорее всего такое не провернуть, так как нет X11.