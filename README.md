## Привет, я cvsqwe

Пишу на Python, C++ и QML. Долго сидел на Linux и делал под него всякое, сейчас перешёл на Windows и занимаюсь ботами.

### Сейчас: [matele](https://github.com/cvsqwe/matele)

Фреймворк для ботов, которые работают сразу в MAX и Telegram. Хендлеры пишутся один раз, а различия между мессенджерами matele берёт на себя. Для MAX есть типизированный клиент ко всему Bot API, модели генерируются из официальной схемы.

```python
from matele import Context, Dispatcher
from matele.max import MaxBot
from matele.telegram import TelegramBot

dp = Dispatcher()

@dp.command("start")
async def start(ctx: Context):
    await ctx.reply(f"Привет! Ты пишешь из {ctx.platform}")

dp.run_polling(MaxBot(MAX_TOKEN), TelegramBot(TG_TOKEN))
```

### Раньше

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/cvsqwe/cove"><img src="https://raw.githubusercontent.com/cvsqwe/cove/main/docs/screens/dashboard.webp" alt="cove"></a>
      <p><a href="https://github.com/cvsqwe/cove"><b>cove</b></a><br>
      Моя сборка для Hyprland: свой шелл на Quickshell, редактор, тема для Firefox и терминал в одном стиле. Цвета подстраиваются под обои.</p>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/cvsqwe/OpenAula"><img src="https://raw.githubusercontent.com/cvsqwe/OpenAula/main/docs/screenshots/lighting.png" alt="OpenAula"></a>
      <p><a href="https://github.com/cvsqwe/OpenAula"><b>OpenAula</b></a><br>
      Подсветка и макросы для клавиатуры Aula F75 под Linux. Около 40 эффектов, рисование по клавишам, настройка из браузера.</p>
    </td>
  </tr>
</table>

Ещё есть [мои старые дотфайлы для Hyprland](https://github.com/cvsqwe/MD4H-My-Dotfiles-For-Hyprland-).
