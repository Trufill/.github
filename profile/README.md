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

Состояние на **11.11.2026**. Доступность котировок и доступность обмена различаются. Срез mainnet и управление — по реестру [contracts](https://github.com/Trufill/contracts) от **03.11.2026** и активации Polygon в [monitor](https://github.com/Trufill/monitor). Живые строки сетей — по публичному [`api.trufill.xyz/status`](https://api.trufill.xyz/status) в день этой сверки.

| Направление | Состояние |
| --- | --- |
| **Base** | Ограниченный mainnet-срез: WETH ↔ native USDC, один hop Uniswap V3, комиссия протокола 0 bps. [Реальный обмен в BaseScan](https://basescan.org/tx/0xc20cf7c51ead32ce7602fd33670c48d36287e37b8ab481972f50b5404f09ca8d). |
| **Polygon PoS** | Ограниченный mainnet-срез: WETH ERC20 → native USDC, один hop Uniswap V3, комиссия протокола 0 bps; отдельный Safe. [Реальный обмен в PolygonScan](https://polygonscan.com/tx/0x9c2d97952c378e999ab45b7623c1778951716423bc1d7d68ba550d2e715e2dbd). |
| **Ethereum / Base / Arbitrum Sepolia** | Три активных тестнета для разработки и проверок. В публичном `/status` на 11.11.2026 у всех трёх `rpc=ok` и `routerWiring=ok`. |
| **BNB Chain / Arbitrum** | Публичный реестр mainnet от 03.11.2026 и `/status` на 11.11.2026 эти сети не включают. |
| **Solana / Jupiter** | Живые котировки WSOL ↔ native USDC. Quote-only: подпись и отправка транзакций не реализованы. |
| **Native Solana / Orca / Squads** | Отдельная реализация сохранена; deployment приостановлен бюджетным ограничением. |

На Base (8453) и Polygon PoS (137) развёрнуты AggregatorRouter, FeeSwitch и ParamTimelock: адреса совпадают, развёртывания разные. Управление — **Safe → ParamTimelock → FeeSwitch**; Safe ещё и получатель комиссии, на Polygon Safe отдельный. Смена комиссии, получателя и владельца FeeSwitch ждёт **2 дня** в ParamTimelock; созревшая заявка истекает через **14 дней**. Sourcify v2: `exact_match` для creation и runtime всех шести развёртываний, проверка **03.11.2026**. В реестре комиссия **0 bps**, потолок байткода — **30 bps**. Более широкий V2-интерфейс не означает, что публичный сервис открывает любую пару. Адреса и доказательства: [contracts](https://github.com/Trufill/contracts).

Строки Solana сохранены с описания **02.10.2026**: публичные `contracts`, `monitor` и `/status` эти направления не фиксируют.

Внешний аудит Trufill не проводился. Работающие срезы Base и Polygon не означают готовность всех сетей: каждое новое направление проходит отдельную техническую приёмку перед выпуском.

## Экосистема и код

| Репозиторий | Роль | Языки и стек |
| --- | --- | --- |
| [**dex-aggregator**](https://github.com/Trufill/dex-aggregator) | Основной DEX: EVM-контракты, gateway, quote engine, проверка исполнения и Jupiter quote-only. | **Solidity · TypeScript · JavaScript**; Foundry, Node.js, viem, Vitest. |
| [**contracts**](https://github.com/Trufill/contracts) | Публичный исходник контрактов исполнения на Base и Polygon, тесты и проверка provenance. | **Solidity**; Foundry. |
| [**monitor**](https://github.com/Trufill/monitor) | Внешний мониторинг продакшна: доступность API, терминала и сайта, снимок точности и управление контрактами на Base и Polygon. | **JavaScript**; Node.js ≥20. |
| [**dex-aggregator-solana**](https://github.com/Trufill/dex-aggregator-solana) | Native Solana-путь с Orca и Squads; отдельная область разработки и выпуска. | **Rust · JavaScript**; Solana, Orca Whirlpools, Squads. |
| [**terminal**](https://github.com/Trufill/terminal) | Пользовательский интерфейс котировок и обмена. | **JavaScript · React**. |
| [**web**](https://github.com/Trufill/web) | Сайт продукта и общая визуальная идентичность. | Веб-интерфейс Trufill. |
| [**.github**](https://github.com/Trufill/.github) | Этот публичный профиль организации. | Markdown · SVG. |

Репозитории разработки сейчас **приватные**: ссылки на код требуют выданного доступа. Публично читаются [**contracts**](https://github.com/Trufill/contracts) и [**monitor**](https://github.com/Trufill/monitor). Ссылка «Документация» ведёт в приватный [dex-aggregator](https://github.com/Trufill/dex-aggregator#документация) (якорь `#документация`) и без выданного доступа открывается как 404; публичное описание контрактов исполнения — README `contracts`. Публичный профиль описывает продукт и его состояние; по интеграции, доступу или сотрудничеству [напишите в Telegram](https://t.me/trufill).

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
