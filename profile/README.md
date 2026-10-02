<p align="center">
  <a href="https://trufill.xyz">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Trufill/.github/main/profile/assets/banner-dark.svg">
      <img src="https://raw.githubusercontent.com/Trufill/.github/main/profile/assets/banner-light.svg" alt="Trufill — маршруты обмена, исполнение в вашем кошельке" width="1200">
    </picture>
  </a>
</p>

<h1 align="center">Маршруты сравниваем мы. Обмен подписываете вы.</h1>

<p align="center">
  Trufill соединяет ликвидность DEX с вашим кошельком.<br>
  Котировка, условия обмена и проверяемый результат — в одном процессе.
</p>

<p align="center">
  <a href="https://swap.trufill.xyz"><img src="https://raw.githubusercontent.com/Trufill/.github/main/profile/assets/buttons/swap.svg" height="38" alt="Открыть терминал"></a>
  <a href="https://trufill.xyz"><img src="https://raw.githubusercontent.com/Trufill/.github/main/profile/assets/buttons/product.svg" height="38" alt="О продукте"></a>
  <a href="https://github.com/Trufill/dex-aggregator#документация"><img src="https://raw.githubusercontent.com/Trufill/.github/main/profile/assets/buttons/docs.svg" height="38" alt="Документация для разработчиков"></a>
  <a href="https://t.me/trufill"><img src="https://raw.githubusercontent.com/Trufill/.github/main/profile/assets/buttons/contact.svg" height="38" alt="Связаться в Telegram"></a>
</p>

<p align="center">
  <a href="https://docs.soliditylang.org/"><img src="https://raw.githubusercontent.com/Trufill/.github/main/profile/assets/languages/solidity.svg" height="20" alt="Solidity 0.8.28"></a>
  <a href="https://www.typescriptlang.org/docs/"><img src="https://raw.githubusercontent.com/Trufill/.github/main/profile/assets/languages/typescript.svg" height="20" alt="TypeScript 5.9.2"></a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript"><img src="https://raw.githubusercontent.com/Trufill/.github/main/profile/assets/languages/javascript.svg" height="20" alt="JavaScript · ESM"></a>
  <a href="https://doc.rust-lang.org/book/"><img src="https://raw.githubusercontent.com/Trufill/.github/main/profile/assets/languages/rust.svg" height="20" alt="Rust · edition 2021"></a>
  <a href="https://nodejs.org/docs/latest-v20.x/api/"><img src="https://raw.githubusercontent.com/Trufill/.github/main/profile/assets/languages/nodejs.svg" height="20" alt="Node.js ≥20"></a>
  <a href="https://react.dev/reference/react"><img src="https://raw.githubusercontent.com/Trufill/.github/main/profile/assets/languages/react.svg" height="20" alt="React 19.2.8"></a>
</p>

---

## Автор

<table>
  <tr>
    <td align="center" width="116">
      <a href="https://github.com/artemmalanin979-create"><img src="https://avatars.githubusercontent.com/u/225334540?s=160&amp;v=4" width="80" height="80" alt="Артём Маланин"></a>
    </td>
    <td>
      <strong>Артём Маланин</strong><br>
      Основатель и разработчик Trufill<br>
      <a href="https://github.com/artemmalanin979-create">GitHub</a> · <a href="https://www.linkedin.com/in/artem-malanin-3a9818420">LinkedIn</a> · <a href="https://x.com/ArtemMalaninDev">X</a> · <a href="https://t.me/trufill">Telegram</a>
    </td>
  </tr>
</table>

## Что такое Trufill

**Trufill — некастодиальный DEX-агрегатор.** Он сравнивает доступные маршруты обмена, готовит транзакцию и позволяет проверить результат по данным блокчейна. Средства остаются под контролем пользователя: обмен требует подписи в его кошельке.

Мы строим продукт вокруг понятных условий исполнения. До подписи пользователь видит маршрут и минимальный выход; контракт должен выполнить этот минимум или откатить обмен. Рыночный результат может отличаться от предварительной котировки.

| Для пользователя | Для разработчика |
| --- | --- |
| **Терминал обмена** — выбрать рынок, получить котировку, проверить условия. | **API и quote engine** — маршруты, доступность источников и журнал котировок. |
| **Собственный кошелёк** — проверить и подписать транзакцию. | **Контрактный роутер** — minimum output, deadline и управление параметрами. |
| **Результат в цепи** — транзакция и полученные токены. | **Проверка исполнения** — связь quote с транзакцией, receipt и изменениями балансов. |

[Открыть терминал](https://swap.trufill.xyz) · [Познакомиться с продуктом](https://trufill.xyz)

## Где мы сейчас

Состояние на **02.10.2026**. Доступность котировок и доступность обмена различаются.

| Направление | Состояние |
| --- | --- |
| **Base** | Ограниченный mainnet-срез: WETH ↔ native USDC, один hop Uniswap V3, комиссия протокола 0 bps. [Реальный обмен в BaseScan](https://basescan.org/tx/0xc20cf7c51ead32ce7602fd33670c48d36287e37b8ab481972f50b5404f09ca8d). |
| **Ethereum / Base / Arbitrum Sepolia** | Три активных тестнета для разработки и проверок. |
| **Polygon / BNB Chain / Arbitrum** | Подготовленные EVM-направления; public swap закрыт, deployment ещё не выполнен. |
| **Solana / Jupiter** | Живые котировки WSOL ↔ native USDC. Quote-only: подпись и отправка транзакций не реализованы. |
| **Native Solana / Orca / Squads** | Отдельная реализация сохранена; deployment приостановлен бюджетным ограничением. |

Внешний аудит Trufill не проводился. Работающий Base-срез не означает готовность всех сетей: каждое новое направление проходит отдельную техническую приёмку перед выпуском.

## Экосистема и код

| Репозиторий | Роль | Языки и стек |
| --- | --- | --- |
| [**dex-aggregator**](https://github.com/Trufill/dex-aggregator) | Основной DEX: EVM-контракты, gateway, quote engine, проверка исполнения и Jupiter quote-only. | **Solidity · TypeScript · JavaScript**; Foundry, Node.js, viem, Vitest. |
| [**dex-aggregator-solana**](https://github.com/Trufill/dex-aggregator-solana) | Native Solana-путь с Orca и Squads; отдельная область разработки и выпуска. | **Rust · JavaScript**; Solana, Orca Whirlpools, Squads. |
| [**terminal**](https://github.com/Trufill/terminal) | Пользовательский интерфейс котировок и обмена. | **JavaScript · React**. |
| [**web**](https://github.com/Trufill/web) | Сайт продукта и общая визуальная идентичность. | Веб-интерфейс Trufill. |
| [**.github**](https://github.com/Trufill/.github) | Этот публичный профиль организации. | Markdown · SVG. |

Репозитории разработки сейчас **приватные**: ссылки на код требуют выданного доступа. Публичный профиль описывает продукт и его состояние; по интеграции, доступу или сотрудничеству [напишите в Telegram](https://t.me/trufill).

## На чьей работе строим

Trufill использует открытые библиотеки и протоколы; благодарим их авторов и сопровождающих.

- [**OpenZeppelin**](https://github.com/OpenZeppelin/openzeppelin-contracts) — контрактные библиотеки EVM.
- [**Uniswap**](https://github.com/Uniswap) — протоколы V3/V2 и основа изолированного дерева V2-пулов.
- [**Jupiter**](https://github.com/jup-ag) — Solana quote API в основном DEX.
- [**Orca**](https://github.com/orca-so/whirlpools) и [**Squads**](https://github.com/Squads-Protocol) — компоненты отдельного native Solana-пути.

Лицензии определяются файлами и зависимостями каждого репозитория. Эти команды указаны как upstream, их участие в команде Trufill не заявляется.

## На связи

По вопросам продукта, интеграции и сотрудничества — [**@trufill в Telegram**](https://t.me/trufill).

<p align="center">
  <a href="https://trufill.xyz"><strong>trufill.xyz</strong></a> ·
  <a href="https://swap.trufill.xyz">Терминал</a> ·
  <a href="https://github.com/Trufill/dex-aggregator#документация">Документация</a> ·
  <a href="https://t.me/trufill">Связаться</a>
</p>
