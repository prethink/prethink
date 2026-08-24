<h1 align="center">Hi there, I'm Ilya 👋</h1>

<p align="center">
  <b>Self-taught .NET developer</b> — I build reusable frameworks, not one-off scripts.<br/>
  Telegram bots, Unity gameplay systems and the plumbing that makes both boring to write.
</p>

<p align="center">
  <a href="https://www.nuget.org/packages/PRTelegramBot/">
    <img src="https://img.shields.io/nuget/dt/PRTelegramBot?style=flat-square&logo=nuget&label=NuGet%20downloads&color=004880" alt="NuGet downloads"/>
  </a>
  <a href="https://github.com/prethink?tab=repositories">
    <img src="https://img.shields.io/badge/focus-C%23%20%2F%20.NET%20%2F%20Unity-5C2D91?style=flat-square" alt="Focus"/>
  </a>
</p>

---

## 🚀 Featured Projects

### 🤖 [PRTelegramBot](https://github.com/prethink/PRTelegramBot) — a framework for Telegram bots on .NET

[![Stars](https://img.shields.io/github/stars/prethink/PRTelegramBot?style=flat-square&color=f5c518)](https://github.com/prethink/PRTelegramBot/stargazers)
[![NuGet](https://img.shields.io/nuget/v/PRTelegramBot?style=flat-square&logo=nuget&color=004880)](https://www.nuget.org/packages/PRTelegramBot/)
[![License](https://img.shields.io/github/license/prethink/PRTelegramBot?style=flat-square)](https://github.com/prethink/PRTelegramBot/blob/master/LICENSE)

Writing a Telegram bot usually means one giant `switch` over `update.Message.Text`.
**PRTelegramBot replaces that switch with attributes** — you mark a method, the framework finds it and routes the update to it.

```csharp
[ReplyMenuHandler("start", "menu")]
public static async Task Start(ITelegramBotClient bot, Update update)
    => await Helpers.Message.Send(bot, update, "Main menu");
```

- 🧭 **Attribute-based routing** — `SlashHandler`, `ReplyMenuHandler`, `InlineHandler`, parameterized commands
- 🧱 **Ready-made UI** — menu/keyboard builders, a date picker calendar, paginated messages
- 🔌 **Real architecture** — middleware pipeline, DI, event bus, background jobs with retries
- 🛰️ **Polling and webhook**, multi-bot in one process, admin/whitelist management, `ILogger` support
- 🎯 **Non-invasive wrapper** — the whole `Telegram.Bot` API stays available, nothing is hidden from you

*Built on Telegram.Bot • .NET 6.0+ • MIT • published on NuGet with SemVer and backward-compatibility guarantees.*

---

### 🎮 [PRUnitySDK](https://github.com/prethink/PRUnitySDK) — the layer every Unity project rewrites

[![Unity](https://img.shields.io/badge/Unity-2022.3%20LTS%2B-000000?style=flat-square&logo=unity)](https://github.com/prethink/PRUnitySDK)
[![Status](https://img.shields.io/badge/status-active%20development-orange?style=flat-square)](https://github.com/prethink/PRUnitySDK)

Every new game starts with the same three days of work: a lifecycle, a pause system, an event bus.
**PRUnitySDK is those three days, already done** — a set of systems designed to be dropped into a project and grown with it.

- 🔄 **`PRMonoBehaviour`** — a base component with an explicit lifecycle and built-in pause awareness
- 📡 **`EventBus`** — typed global events, no more `FindObjectOfType` spaghetti
- ⏸️ **`PauseManager` + `PRTime`/`PRTimeScale`** — several independent kinds of pause (logic, audio, UI) instead of one global `Time.timeScale`
- 🚩 **`FlagsSystem`** — shared, conflict-free state control over a single object
- 🎁 **Gameplay modules** — entities, items, resources, rewards, progression
- 🧩 **Bootstrap-scene initialization**, optional **Zenject** and **YG2** integrations

*Unity 2022.3 LTS+ • Newtonsoft Json for Unity + DOTween • installed as a Git submodule.*

---

### 🔫 [Cs2Telegram](https://github.com/prethink/Cs2Telegram) — a CS2 server inside a Telegram chat

[![Stars](https://img.shields.io/github/stars/prethink/Cs2Telegram?style=flat-square&color=f5c518)](https://github.com/prethink/Cs2Telegram/stargazers)

A plugin that pipes a Counter-Strike 2 server into Telegram: server events reach the chat, and the chat reaches the server back. Admin without RCON and without opening the game.

---

## 🛠️ Tech Stack

**Core**

![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-5C2D91?style=for-the-badge&logo=dotnet&logoColor=white)
![Unity](https://img.shields.io/badge/Unity-000000?style=for-the-badge&logo=unity&logoColor=white)
![Telegram](https://img.shields.io/badge/Telegram%20Bot%20API-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)

**Web**

![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)
![React](https://img.shields.io/badge/React-20232a?style=for-the-badge&logo=react&logoColor=61DAFB)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

**AI-assisted development**

![Claude](https://img.shields.io/badge/Claude-D97757?style=for-the-badge&logo=claude&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude%20Code-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![Codex](https://img.shields.io/badge/OpenAI%20Codex-412991?style=for-the-badge&logo=openai&logoColor=white)
![ChatGPT](https://img.shields.io/badge/ChatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white)

**Tools**

![Visual Studio](https://img.shields.io/badge/Visual%20Studio-5C2D91?style=for-the-badge&logo=visualstudio&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-0078d7?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![NuGet](https://img.shields.io/badge/NuGet-004880?style=for-the-badge&logo=nuget&logoColor=white)

---

## 📫 Contacts

<p align="center">
  <a href="https://t.me/prethink"><img src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram"/></a>
  <a href="mailto:ilia-samarin@bk.ru"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>
