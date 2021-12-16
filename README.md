[![Build status](https://ci.appveyor.com/api/projects/status/0qbvl5e74hn8lek7?svg=true)](https://ci.appveyor.com/project/ajoq/ajs-homeworks-11-symbols-iterators-generators-11-2)

# Домашнее задание к лекции «Символы, итераторы, генераторы»

**Важно**: код должен проходить ESLint без ошибок.

**Важно**: на задачи данного раздела писать авто-тесты не нужно.

---

## Символы и генераторы

### Легенда

Реализовывать итераторы [задание 1](https://github.com/ajoq/ajs-homeworks_11-symbols-iterators-generators_11.1-symbols-iterators) не так уж здорово, правда? Давайте посмотрим, как нам могут помочь генераторы при переборе.

### Описание

Используйте следующую заготовку для организации перебора класса `Team`:
```javascript
class Team {
  ...
  *[Symbol.iterator]() {
    // это генератор
    // и здесь есть доступ к this
    // остаётся лишь правильно написать yield
  }
}
```