---
start: false
title: "Живе кодування – це навичка"
block: "Формування навичок викладання"
teaching: 20
exercises: 50
questions:
- "Чому ми навчаємо програмуванню за допомогою спільного живого кодування?"
objectives:
- «Поясніть переваги та обмеження спільного живого кодування».
- «Підсумуйте ключові речі, які варто та чого не варто робити в процесі спільного живого кодування».
- «Продемонструйте кодування в реальному часі».
keypoints:
- «Кодування в реальному часі змушує інструктора викладати повільніше».
- «Програмування дає учням постійну практику та зворотний зв’язок».
- «Помилки, допущені під час спільного кодування в реальному часі, є цінними можливостями для навчання».
---

Одним із наріжних каменів викладання Carpentries є живе
кодування: *інструктори не використовують слайди*, а опрацьовують матеріал уроку,
набираючи код або інструкції, яким слідують учасники семінару.
У цьому розділі пояснюється, як це працює, чому ми це використовуємо та
даються загальні поради щодо ефективної спільної презентації кодування в реальному часі. Завершимо 
цей розділ самостійним тренуванням з наданням відгуку один одному.

## Чому сумісне живе кодування?

Ми не використовуємо слайди на уроках.
Натомість інструктори підключають свій ноутбук до проектора
і працюють на уроці,
набираючи код,
переформатовуючи дані
та розповідаючи про перебіг виконання поточних завдань.
Це називається ["живе кодування"](https://en.wikipedia.org/wiki/Live_coding).
Однак інструктор не виконує живе кодування у вакуумі.
Важливо, що слухачів активно заохочують
«кодувати разом» з інструктором.
Ми називаємо практику, коли інструктор виконує  живе кодування разом зі слухачами, «сумісним живим кодуванням» або, менш формально, «сеансами кодування».

> ## Вгору та вниз
>
> Перелічіть деякі переваги та проблеми сумісного живого кодування
> як з точки зору слухача, так і з точки зору викладача
> в Etherpad.
>
> Це обговорення має тривати близько 10 хвилин.
>
>> ## Рішення
>> Деякі переваги:
>>
>> * Спостерігати за написанням програми є більш переконливим, ніж
>> спостерігати за тим, як хтось гортає слайди, які представляють фрагменти того самого коду.
>> * Це дає можливість інструкторам краще реагувати на "що, якщо?" запитання.
>> Якщо слайд-презентацію порівняти  із залізничною колією,
>> то сумісне живе кодування дозволяє інструкторам вийти на узбіччя та слідувати інтересам своїх слухачів.
>> * Латеральна передача знань: сумісне живе кодування кодування полегшує передачу [неявних знань](http://jonudell.net/udell/2006-09-19-screencasting-of-tacit-knowledge.html) — люди дізнаються більше ніж ми вважали, 
>> спостерігаючи за тим, як інструктори щось роблять.
>> * Це сповільнює інструктора:
>> якщо йому доводиться вводити програму,
>> він може рухатися лише вдвічі швидше, ніж слухачі,
>> а не в десять разів швидше, ніж він міг б зі слайдами.
>> * Слухачі бачать помилки викладачів *і як їх діагностувати та виправляти*.
>> Новачки витрачатимуть на це більшу частину свого часу,
>> але це є відсутнім у більшості підручників.
>>
>> Деякі проблеми:
>>
>> * Це вимагає від інструкторів здатності імпровізувати, коли щось йде не так, або коли слухачі
>> мають запитання, які прямо не розглянуті в тексті уроку.
>> * Слухачам може бути важко слухати та набирати код одночасно через
>> *ефект роздвоєння уваги* ми
>> [обговорювали це раніше]({{ page.root }}{% link _episodes/05-memory.md %}#why-guided-practice-is-important).
>> Ось чому 
>> дуже важливо, щоб інструктори спочатку пояснили, що вони збираються робити, а потім
>> сказати, який код вони набирають, а потім
>> знову пояснили, що вони зробили.
>> * Інструкторам може знадобитися трохи практики
>> звикнути думати вголос під час кодування перед аудиторією.
>>
> {: .solution}
{: .challenge}

Живе кодування добре вписується в практичну модель зворотного зв’язку, яку ми обговорювали – надаючи
слухачам постійні можливості для практики (щоразу, коли вони набирають рядок коду)
і постійний зворотний зв'язок (цей код або працює, або генерується повідомлення про помилку). 
Однак важливо пам’ятати, що зворотній зв’язок не є корисним, якщо ви йогоне розумієте.
Багато повідомлень про помилки незрозумілі та написані не для новачків. Продовжуйте використовувати стратегії для визначення помилок, про які
[ми дізналися раніше]({{ page.root }}{% link _episodes/09-mindset.md %}#errors-are-essential-to-learning), щоб переконатися, що цей тип зворотного зв’язку буде корисним для слухачів.

> ## Порівнювати і протиставляти
>
> Перегляньте це [перше демо-відео про живе кодування] [live-coding-bad]
> і це [друге демо-відео][live-coding-good]
> у групі, а потім узагальніть свої відгуки про обидва відео в Etherpad.
> Використайте рубрику 2x2 для зворотного зв’язку, яку ми обговорювали раніше.
>
> У відео пояснюється цикл `for` оболонки bash,
> передбачається, що слухачі знають, як використовувати змінні,
> команду `head` і вміст `basilisk.dat unicorn.dat`
> файлів.
>
> Примітка: Іноді відео погато чути в кімнаті . Увімкнення субтитрів натисканням кнопки cc покращить доступність цих відео.
>
> Ця вправа та обговорення мають тривати приблизно 15 хвилин.
>
> > ## Рішення
> > Інструктор проведе обговорення відео та ваші відгуки про них,
> > Переконайтеся, що пункти десяти найкращих порад, наведених нижче, виконані.
> >
> {: .solution}
{: .challenge}

## Десять найкращих порад щодо сумісного живого кодування на семінарі
1. **Встаньте та пересувайтеся кімнатою, якщо це можливо.** Це робить процес більш інтерактивним і менш монотонним. Використовуйте мікрофон, якщо він доступний, щоб людям з проблемами слуху було легше почути вас.
2. **Викладайте повільно.** Для кожної команди, яку ви вводите, для кожного слова коду, яке ви пишете, кожного пункту меню чи кнопки веб-сайту, яку ви натискаєте, промовляйте вголос, що ви робите під час цієї дії. Потім наведіть вказівник на команду тазображення на екрані та пройдіть через це вдруге. Це сповільнює вас і дозволяє слухачам копіювати те, що ви робите, або наздоганяти. Не копіюйте та не вставляйте код.
3. **Віддзеркалюйте середовище вашого слухача.** Спробуйте створити середовище, яке буде максимально схожим на те, що мають ваші слухачі, щоб зменшити когнітивне навантаження. Уникайте використання комбінацій клавіш.
4. **Використовуйте екран проектора розумно.** Використовуйте великий шрифт і розгорніть вікно. Чорний шрифт на білому фоні працює краще, ніж світлий шрифт на темному тлі. Коли нижня частина екрану проектора знаходиться на тій самій висоті або нижче голів слухачів, люди позаду не зможуть бачити нижню частину. Намалюйте нижню частину вікна(-й), щоб компенсувати це. Зверніть увагу на освітлення (не надто темне, без світла безпосередньо на/над екраном доповідача) і, якщо необхідно, переставте столи так, щоб усі слухачі могли бачити екран, а помічники могли легко дістатися до всіх слухачів.
5. **Використовуйте ілюстрації**, щоб допомогти слухачам зрозуміти та систематизувати матеріал. Ви також можете створювати ілюстрації на дошці під час проходження матеріалу. Це дозволяє вам будувати діаграми, роблячи їх все більш складними паралельно з матеріалом, який ви викладаєте. Це допомагає слухачам зрозуміти матеріал, робить семінар більш жвавим і також привертає увагу слухачів до вас.
6. **Turn off notifications** on your laptop and phone.
7. **Stick to the lesson material.** The core Carpentries lessons are developed collaboratively by many instructors and tried and tested at many workshops.  This means they are very streamlined - which is great when you start teaching them for the first time.  It may be tempting to deviate from the material because you would like to show a neat trick, or demonstrate some alternative way of doing something.  Don't do this, since there is a fair chance you'll run into something unexpected that you then have to explain.  If you really want to use something outside of the material, try it out thoroughly before the workshop: run through the lesson as you would during the actual teaching and test the effect of your modification.
Some instructors use printouts of the lesson material during teaching. Others use a second device (tablet or laptop) when teaching, on which they can view their notes and the Etherpad session.  This seems to be more reliable than displaying one virtual desktop while flipping back and forth to another.
8. **Leave no learner behind.** Use sticky notes, see below, to gauge learners' progress and understanding.
9. **Embrace mistakes.** No matter how well prepared you are, you will make mistakes. This is OK! Use these opportunities to do [error framing]({{ page.root }}{% link _episodes/09-mindset.md %}#errors-are-essential-to-learning) and to help your learners learn the art of troubleshooting.
10. **Have fun!** It's OK to use humor and improvisation to liven up the workshop. This becomes easier when you are more familiar with the material, and more relaxed. Start small, even just saying 'that was fun' after something worked well is a good start.

## Sticky Notes
Give each learner two sticky notes of different colours, e.g., yellow and blue.
If someone has completed an exercise, they put the blue sticky note on their laptop;
if they run into a problem and need help, the put up the yellow one.  This is better
than having people raise their hands because:

*  it's more discreet (which means they're more likely to actually do it),
*  they can keep working while their flag is raised, and
*  the instructor can quickly see from the front of the room what state the class is in.

Sometimes a yellow sticky involves a technical problem that takes a bit
more time to solve.  To prevent this issue slowing down the whole
class too much, you could use the occasion to take the small break you
had planned to take a bit later, giving the helper(s) time to fix the
problem.

Remind learners frequently about using their sticky notes, or they (and you) will forget.

> ## Accessibility of Sticky Notes
> We strongly encourage you to get sticky notes in colors other than red and green, 
> as we have found that some learners (not to mention helpers and instructors!) 
> may have colorblindness and thus cannot properly ask for/give help this way. 
> Alternate ideas are to use differently-shaped sticky notes (stars and squares, 
> thumbs up that can be turned into thumbs down stickies), or to use one sticky note 
> as a flag for help.
{: .callout}

> ## Practice Teaching
>
> Teach 3 minutes of your chosen lesson episode using live coding to one or two
> fellow trainees, then swap and watch while the other person(s) live codes for
> you. (For this exercise, your peers will not "code-along", but will instead observe and give feedback.)
>
> Explain in advance to your fellow trainee(s) what you will be teaching
> and what the learners you teach it to are expected to be familiar with.
>
> **Don't record this exercise.** Give each other feedback
> using the 2x2 rubric we discussed previously and enter the feedback
> you received in the Etherpad.
>
> This exercise should take about 25 minutes.  
{: .challenge}


[live-coding-bad]: https://youtu.be/bXxBeNkKmJE
[live-coding-good]: https://youtu.be/SkPmwe_WjeY

