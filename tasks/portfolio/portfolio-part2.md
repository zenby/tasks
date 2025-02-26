## portfolio

### Часть 2. Адаптивная вёрстка

В этой части задания адаптируем ранее сверстанную страницу для планшетов и мобильных устройств.  
На разрешении 768рх ставится задача совпадения вёрстки с [макетом](https://www.figma.com/file/YcEST7ugdfJ7d28jSNN2Oh/Portfolio-adaptive).  
На остальных разрешениях до 320рх включительно достаточно обеспечить отсутствие горизонтальной полосы прокрутки.  
Также на этом этапе добавляем в вёрстку адаптивное меню, при создании которого используется js-код.

В первую очередь ознакомьтесь с [описанием и требованиями задания](portfolio.md)

## Требования к вёрстке
1. Вёрстка соответствует макету. Ширина экрана 768px +48
   - блок `<header>` +6
   - секция `hero` +6
   - секция `skills` +6
   - секция `portfolio` +6
   - секция `video` +6
   - секция `price` +6
   - секция `contacts` +6
   - блок `<footer>` +6 
2. Ни на одном из разрешений до 320px включительно не появляется горизонтальная полоса прокрутки +15
   - нет полосы прокрутки при ширине страницы от 1440рх до 768рх +5
   - нет полосы прокрутки при ширине страницы от 768рх до 480рх +5
   - нет полосы прокрутки при ширине страницы от 480рх до 320рх +5
3. На ширине экрана 768рх и меньше реализовано адаптивное меню +22
   - при ширине страницы 768рх панель навигации скрывается, появляется бургер-иконка +2   
   - при нажатии на бургер-иконку плавно появляется адаптивное меню, бургер-иконка изменяется на крестик +4
   - адаптивное меню по ширине и высоте занимает весь размер экрана, вёрстка меню соответствует макету +4
   - при нажатии на крестик адаптивное меню плавно скрывается, крестик превращается в бургер-иконку +4
   - бургер-иконка, которая при клике превращающается в крестик, создана при помощи css-анимаций без использования изображений +2
   - ссылки в адаптивном меню работают, обеспечивая плавную прокрутку по якорям +2
   - при клике по ссылке в адаптивном меню адаптивное меню плавно скрывается, крестик превращается в бургер-иконку +4 

## Критерии оценки

**Максимальная оценка за задание 75 баллов**  

Баллы за пункты требований указаны в разделе [Требования к вёрстке](#требования-к-вёрстке)

Для удобства проверки выведите в консоль браузера самооценку своего проекта по пунктам с указанием баллов за каждый выполненный вами пункт.

Разница между максимальной оценкой за задание (75 баллов) и максимально возможным количеством баллов за выполнение всех пунктов требований (85 баллов) позволит сгладить возможные ошибки проверяющих в ходе кросс-чека, неточности в описании задания, разное понимание требований задания проверяющим и проверяемым.

## Особенности проверки адаптивности в DevTools
1. Открываем инструменты разработчика
   - для этого нажимаем клавишу `F12` или кликаем правой кнопки мыши и выбираем в появившемся меню пункт `Посмотреть код`
   - в правом верхнем углу панели инструментов разработчика кликаем на иконку `Toggle device toolbar`
   - на верхней панели выбираем `Responsive`
2. Убедитесь, что в режиме `Responsive` нет вертикальной полосы прокрутки (она отсутствует по умолчанию). Если полоса прокрутки есть, её нужно убрать. Для этого
   - в верхней панели device toolbar переключите тип устройства с `Desktop` на `Mobile` 
   - если тип устройства не отображается, в верхней панели device toolbar нажмите на три точки справа и выберите `Add device type` 
2. Выставляем ширину экрана на требуемую по ТЗ - 768рх, при которой будем проверять адаптивность. Если видим, что страница проверяемого сайта не перестроилась, или справа осталась белая полоса, может понадобиться обновить страницу несколько раз
3. Проверяем вёрстку на соответствие макету
4. При необходимости проверить адаптивность на разных разрешениях, плавно изменяем ширину экрана в DevTools от максимума (1440рх) до минимума (320рх), убеждаемся в отсутствии горизонтальной полосы прокрутки на всех разрешениях. Если появилась полоса прокрутки или белое поле справа, попробуйте обновить страницу, возможно, вёрстка не перестроилась.

## Особенности проверки вёрстки на соответствие макету
- допускается отклонение вёрстки от макета до 10px по горизонтали и вертикали, если соблюдается визуальное сходство вёрстки и макета
- разрешены и даже приветствуются правки размеров и расположения криво нарисованных блоков
- в качестве инструмента для проверки соответствия вёрстки макету используйте расширение [PerfectPixel](https://chrome.google.com/webstore/detail/perfectpixel-by-welldonec/dkaagdgjmgdmbnecmcefdhjekcoceebi?hl=ru)
- при проверке вёрстки при помощи расширения PerfectPixel в первую очередь убедетесь, что в расширении выставлен масштаб 1, в браузере и операционной системе - масштаб 100%
- если разрешение экрана 1440рх и больше, для проверки вёрстки на соответствие макету достаточно вручную выставить макет по верхнему левому углу направляющих
- если разрешение экрана меньше 1440рх, для проверки используем device toolbar браузера Google Chrome в режиме responsive
- каждый блок и секция рассматриваются по раздельности, т.е. недочеты предыдущего блока не переносятся на следующий, а при переходе проверки на следующий блок, мы его выравниваем с наложенным изображением
- относительно текста проверяем его выравнивание по левому краю, отступы до границы блока. Размеры текста проверяются только по высоте. Отличие в ширине слов и отступах между буквами при сопоставлении макета и вёрстки не считается ошибкой, если используется правильный шрифт с правильно указанными свойствами