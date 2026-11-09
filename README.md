## Hi, I'm cvsqwe

I write Python, C++ and QML. Spent a long time on Linux building stuff for it, now I'm on Windows and mostly doing bots.

### Now: [matele](https://github.com/cvsqwe/matele)

A framework for bots that run on MAX and Telegram at the same time. You write handlers once and matele deals with the differences between the messengers. For MAX there's a typed client for the whole Bot API, with models generated from the official schema.

```python
from matele import Context, Dispatcher
from matele.max import MaxBot
from matele.telegram import TelegramBot

dp = Dispatcher()

@dp.command("start")
async def start(ctx: Context):
    await ctx.reply(f"Hi! You're writing from {ctx.platform}")

dp.run_polling(MaxBot(MAX_TOKEN), TelegramBot(TG_TOKEN))
```

### Before

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/cvsqwe/cove"><img src="https://raw.githubusercontent.com/cvsqwe/cove/main/docs/screens/dashboard.webp" alt="cove"></a>
      <p><a href="https://github.com/cvsqwe/cove"><b>cove</b></a><br>
      My Hyprland setup: a custom Quickshell shell, an editor, a Firefox theme and a terminal, all in one style. Colors follow the wallpaper.</p>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/cvsqwe/OpenAula"><img src="https://raw.githubusercontent.com/cvsqwe/OpenAula/main/docs/screenshots/lighting.png" alt="OpenAula"></a>
      <p><a href="https://github.com/cvsqwe/OpenAula"><b>OpenAula</b></a><br>
      Lighting and macros for the Aula F75 keyboard on Linux. Around 40 effects, per-key painting, configured from the browser.</p>
    </td>
  </tr>
</table>

There are also [my old Hyprland dotfiles](https://github.com/cvsqwe/MD4H-My-Dotfiles-For-Hyprland-).
