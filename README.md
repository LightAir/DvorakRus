[![warning](https://img.shields.io/badge/warning-Make%20a%20backup%20before-yellow.svg)]() 

# DvorakRus

Русская, фонетическая раскладка Дворак.

![dvorak layout](https://github.com/LightAir/DvorakRus/blob/master/img/dvorak_layout_ru.png)

## Установка
archlinux & ubuntu. На других не проверялось.

**Перед установкой настоятельно рекомендую выполнить бекап заменяемых файлов!**

Установка производится путём подмены некоторых системных файлов. Что и куда копируется можно посмотреть в replace.sh

```
cd ~/ && git clone https://github.com/LightAir/DvorakRus.git && cd DvorakRus/ && chmod +x replace.sh
sudo ./replace.sh
```

Если вы используете малопопулярную wm, то можете установить раскладку путём добавления
в файл автозагрузки строки:

```setxkbmap "us,ru,dvorak,ru" -variant ",,,rud" -option "grp:alt_shift_toggle"```

В данном примере на **alt+shift** назначено переключение по 4 раскладкам:
```us, ru, dvorak, dvorak ru phonetic```

Настройка раскладки в KDE показана тут http://softroot.ru/all/archlinux-dvorak-i-klaviatura-dns/
