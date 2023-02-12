# ZX-to-JPEG
Мой [хакатон-проект](https://bolknote.ru/all/bessonny-hakaton/) по превращению спектрумовских электронных журналов ZX-Форум в просматриваемый вид.

В проекте два файла.

Первый — `make_screenshots` работает только под «МакОСью» (из-за используемого AppleScript в коде) и нужен для того, чтобы делать
скриншоты [из эмулятора](http://zx.researcher.su) «Спектрума». Он сам умеет нажимать на кнопку листания, убирать дублирующиеся скриншоты и понимает
когда надо прекратить листать. Для работы требует утилиту `cliclick`, которую на «Маке» можно поставить через «брю» (`brew install cliclick`).

Второй файл `convert_to_jpegs` собирает из наделанных скриншотов один или несколько файлов JPEG. Так как высота файла JPEG не может быть больше 65535
пикселей, могут получится несколько файлов. Файлы можно найти по маске `out*.jpg`.

Получившиеся файлы я обернул в небольшой сайт, ссылку выложку, когда у меня дооптимизируюься жпеги.
