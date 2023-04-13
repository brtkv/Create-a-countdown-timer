# Create-a-countdown-timer
 how to create interactive elements that count time - timers

В коді ви можете побачити змінну  deadline , куди записується час закінчення таймеру.
Далі йде функція getTimeRemaining , де ми маємо змінну t в котру записується час: Date.parse(endtime) - Date.parse(new Date()), тобто різниця між кінцевим часом закнічення таймеру і теперішнім.
В змінні seconds, minutes, hours ми вираховуємо і вносимо округлений результат математ дій. 
Далі функція буде повертати ключ - значення: 'total': t, 'hours': hours,'minutes':minutes,'seconds' : seconds.
Функція setClock з змінними (id,endtime ) , в котру ми витягуємо за допомогою метода getElementById,querySelector в змінні seconds, minutes, hours , секунди, хвилини і години з хтмл документа , де вказаний id timer.
Функція function updateClock. Тут ми додаємо 0 перед значеннями, які складаються з однієї цифри. А якщо дата вже пройшла, буде виводитись  '00'. 
Вкінці ми бачимо  setClock('timer',deadline). В цю функцію ми підключаємо 'timer'- з хтмл документа,
deadline - та змінна, в яку ми записували  час закінчення таймеру.
