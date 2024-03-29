Liftcord это современная, простая в использовании, многофункциональная и асинхронная готовая оболочка API для Discord, написанная на Python и предназначенная для русскоговорящего СНГ сообщества.

Ключевые особенности
-------------

- Современное Python использование ``async`` и ``await``.
- Точная обработка скорости.
- Оптимизация скорости и памяти.

Установка
----------

**Python 3.8 или выше обязательно**

Чтобы установить библиотеку, вы можете выполнить следующие действия:


.. code:: sh

    $ git clone https://github.com/liftcord/liftcord/
    $ cd liftcord


Необязательные библиотеки
~~~~~~~~~~~~~~~~~~


* libffi-dev (или ``libffi-devel`` на некоторых системах)
* python-dev (например: ``python3.6-dev`` для Python 3.6)


Быстрый пример
~~~~~~~~~~~~~

.. code:: py

    from liftcord.ext import commands


    bot = commands.Bot(command_prefix='&')

    @bot.command(name = 'лифткорд')
    async def say_lc(ctx):
        await ctx.reply('ЛифтКорд!')

    bot.run('TOKEN')


Вы можете найти больше примеров в директории примеров.

**ПРИМЕЧАНИЕ:** Не рекомендуется оставлять свой ТОКЕН непосредственно в коде, так как это позволяет любому, у кого он есть, получить доступ к вашему боту. Если вы намерены сделать свой код общедоступным, `вы должны надежно хранить его <https://github.com/liftcord/liftcord/blob/master/examples/secure_token_storage.py/>`_.

Ссылки
------

- `Документация <https://liftcord.readthedocs.io/en/latest/>`_
- `Официальный Дискорд сервер <https://discord.gg/------->`_
- `Discord API <https://discord.gg/discord-api>`_
