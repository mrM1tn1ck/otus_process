### OTUS Linux Professional Lesson #13 | Process

## Домашнее задание
```
Работаем с процессами
Задания на выбор
1) написать свою реализацию ps ax используя анализ /proc
- Результат ДЗ - рабочий скрипт который можно запустить
2) написать свою реализацию lsof
- Результат ДЗ - рабочий скрипт который можно запустить
3) дописать обработчики сигналов в прилагаемом скрипте, оттестировать, приложить сам скрипт, инструкции по использованию
- Результат ДЗ - рабочий скрипт который можно запустить + инструкция по использованию и лог консоли
4) реализовать 2 конкурирующих процесса по IO. пробовать запустить с разными ionice
- Результат ДЗ - скрипт запускающий 2 процесса с разными ionice, замеряющий время выполнения и лог консоли
5) реализовать 2 конкурирующих процесса по CPU. пробовать запустить с разными nice
- Результат ДЗ - скрипт запускающий 2 процесса с разными nice и замеряющий время выполнения и лог консоли
```

#### Написать свою реализацию ps ax
```
PID       USER      COMM                                                        STAT RSS
1         root      /sbin/init                                                  S    13396
2         root      /init                                                       S    1500
44        root      /usr/lib/systemd/systemd-journald                           S    19504
87        root      /usr/lib/systemd/systemd-udevd                              S    6036
131       systemd-resolve/usr/lib/systemd/systemd-resolved                      S    11844
132       systemd-timesync/usr/lib/systemd/systemd-timesyncd                    S    6540
167       root      /usr/sbin/cron-f-P                                          S    2680
179       root      /usr/lib/systemd/systemd-logind                             S    8604
183       root      /usr/libexec/wsl-pro-service-vv                             S    22632
201       root      /sbin/agetty-o-p -- \u--noclear-linux                       S    1188
320       root      /init                                                       S    120
322       root      /bin/login-f                                                S    4544
362       mrm1tn1k  /usr/lib/systemd/systemd--user                              S    11204
363       mrm1tn1k  (sd-pam)                                                    S    1720
378       mrm1tn1k  -bash                                                       S    5148
449       mrm1tn1k  ./wslconnectwsl-F-p127.0.0.1:22017                          S    2324
450       mrm1tn1k  -bash                                                       S    5484
691       polkitd   /usr/lib/polkit-1/polkitd--no-debug                         S    7152
1799      root      /usr/lib/postfix/sbin/master-w                              S    4932
```