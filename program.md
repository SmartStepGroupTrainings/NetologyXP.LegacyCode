# XP. Рефакторинг legacy кода. Базовые приемы.
  * Практические занятия по UnitTesting (курс Нетологии http://netology.ru/programs/xp)
  * https://github.com/SmartStepGroupTrainings/NetologyXP.LegacyCode

## План
1. Определение legacy кода. Код, которые не прошел тесты.
2. Зачем менять код?
    - Добавить фичу
    - Починить баг
    - Улучшить дизайн
    - Оптимизировать использовать ресурсов
3. Книга Michael Feathers "Working effectively with legacy code"
4. Способы изменения legacy кода
    - Edit & Pray
    - Cover & Modify
5. Юнит-тесты и препятствия (legacy code dilemma)
    - Change code <> Write Tests
6. Алгоритм изменения легаси кода
    - Identify change points
    - Find test points
    - Break dependencies
    - Write tests
    - Make changes -> refactor
7. Определение шва\точки стыка (Seam)
    - Place where you can alter behavior without editing code in that place.
8. Базовые приемы
    - Network
        - Extract method
        - Pass parameter isTestMode
        - create function postReceiveError() in global scope
    - BarcodeScanner
        - Задокументировать результат (вызвать метод и скопировать output)
        - Start writing unit test
        - Extract print(line)
        - Add print implementation for testing
        - Finish Unit test
        - Починить баг\добавить новое поведение и убедиться, что мы ничего не сломали.   
9. Домашнее задание