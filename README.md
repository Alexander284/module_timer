# module_timer
1. Для использования модуля необходимо установить npm пакеты:
   npm init -y
   npm install webpack webpack-cli --save-dev

2. Важно обращаться внимания на пути в файле webpack.config.js

3. Так же в проекте должен лежать файл script.js с содержимым:

   "use strict";
   import timer from './timer';
   window.addEventListener('DOMContentLoaded', () =>{
      timer('.timer', '2021-04-20');
   });

   В файле timer.js в главную функцию передаются 2 аргумента ('.timer', '2021-04-20') id - родительский класс таймера
   и deadline (говорит само за себя).

4. Чтобы собрать с помощью webpack, использовать команду: npx webpack.
