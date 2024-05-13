Приветствуются все виды изменений. Не стесняйтесь предлагать броские и смешные названия для существующих примеров. Цель - сделать эту коллекцию как можно более интересной для чтения. Вот несколько способов, с помощью которых вы можете внести свой вклад,

- Если вы заинтересованы в переводе проекта на другой язык (некоторые люди уже делали это в прошлом), пожалуйста, не стесняйтесь открыть тему и дайте мне знать, если вам нужна какая-либо помощь.
- Если изменения, которые вы предлагаете, значительны, то создание issue перед внесением изменений будет оценено по достоинству. Если вы хотите поработать над issue (это очень рекомендуется), выразите свою заинтересованность и вы будете назначены исполнителем.
- Если вы добавляете новый пример, настоятельно рекомендуется создать issue, чтобы обсудить ее перед отправкой изменений. Для добавления нового примера вы можете использовать следующий шаблон:

<pre>
### ▶ Какое-то причудливое название. *
* в конце названия означает, что пример был добавлен недавно.

```py
# Подготовка кода.
# Подготовка к волшебству...
```

**Вывод (версия Python):**
```py
>>> triggering_statement
Вероятно, неожиданный вывод

```
(Необязательно): Одна строка, описывающая неожиданный вывод.

#### 💡 Объяснение:
* Краткое объяснение того, что происходит и почему это происходит.
  ```py
  Подготовка примеров для пояснения (при необходимости)
  ```

  **Вывод:**
  ```py
  >>> trigger # пример, облегчающий понимание магии
  # обоснованный вывод
  ```
</pre>

Несколько моментов, которые стоит учитывать при написании примера,

- Если вы решили отправить новый пример без создания issue и обсуждения, пожалуйста, проверьте проект, чтобы убедиться, что в нем уже нет похожих примеров.
- Старайтесь быть последовательными в именах и значениях, которые вы используете для переменных. Например, большинство имен переменных в проекте имеют вид `some_string`, `some_list`, `some_dict` и т.д. Вы увидите много `x` для однобуквенных имен переменных, и `"wtf"` в качестве значений для строк. В проекте нет строгой схемы, как таковой, но вы можете взглянуть на другие примеры, чтобы понять суть.
- Старайтесь быть как можно более креативными, чтобы добавить элемент "сюрприза" во время подготовки примеров. Иногда это может означать написание фрагмента, который здравомыслящий программист никогда бы не написал.
- Также не стесняйтесь добавлять свое имя в список [контрибьюторов](/CONTRIBUTORS.md).

**Некоторые часто задаваемые вопросы**

    Что это такое после каждого заголовка сниппета (###) в README: <!-- ID примера: 30f1d3fc-e267-4b30-84ef-4d9e7091ac1a --->? Нужно ли его добавлять вручную или можно игнорировать при создании новых сниппетов?

Это случайный UUID, он используется для идентификации примеров в нескольких переводах проекта. Как контрибьютор, вы не должны беспокоиться о том, как он используется, вы просто должны добавлять новый случайный UUID к новым примерам в этом формате.

    Куда следует добавлять новые сниппеты? В начало/в конец раздела?

При определении порядка учитывается множество факторов (зависимость от других примеров, уровень сложности, категория и т.д.). Я бы предложил просто добавить новый пример в конец раздела, который вы считаете более подходящим (или просто добавить его в раздел "Разное"). О его порядке можно будет позаботиться в будущих редакциях.

    В чем разница между разделами (первые два очень похожи)?

Раздел "Напрягите мозг" содержит более надуманные примеры, с которыми вы не столкнетесь в реальной жизни, в то время как раздел "Скользкие склоны" содержит примеры, с которыми можно чаще сталкиваться при программировании.

    Перед оглавлением написано, что для его создания использовался markdown-toc -i README.md --maxdepth 3. Пакет pip markdown-toc не содержит ни флагов -i, ни --maxdepth. Какой пакет имеется в виду, или какая версия этого пакета?
    Должна ли новая запись в оглавлении для фрагмента быть создана с помощью вышеуказанной команды или вручную (в случае, если вышеуказанная команда делает больше, чем просто добавляет запись)?

Мы используем пакет [markdown-toc](https://www.npmjs.com/package/markdown-toc) npm для создания ToC (содержание). Однако у него есть некоторые проблемы со специальными символами (не уверен, что они уже исправлены). Чаще всего я просто вставляю ссылку toc вручную в нужное место. Инструмент удобен, когда мне нужно сделать большую перестановку, в остальных случаях просто обновлять toc вручную удобнее.

Если у вас есть вопросы, не стесняйтесь спрашивать в [issue](https://github.com/satwikkansal/wtfpython/issues/269) (спасибо [@LiquidFun](https://github.com/LiquidFun) за ее создание).