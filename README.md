# 🏗 Scaffold-ETH 2

<h4 align="center">
  <a href="https://docs.scaffoldeth.io">Documentation</a> |
  <a href="https://scaffoldeth.io">Website</a>
</h4>

🧪 Набор инструментов для разработки децентрализованных приложений в сети Ethereum. 
Создан для легкого создания и размещения смарт-контрактов, быстрой разработки UI для взаимодействия с ними. 

⚙️ Использует фреймворки NextJS, RainbowKit, Hardhat, Wagmi, and Typescript.

- ✅ **Горячая перезагрузка контракта**: Фронтенд приложения автоматически реагирует на изменения в исходном коде смарт-контракта.
- 🪝 **[Хуки](https://docs.scaffoldeth.io/hooks/)**: Коллекция оберток вокруг React хуков [wagmi](https://wagmi.sh/) упрощает взаимодействие с контрактами. 
- 🧱 [**Компоненты**](https://docs.scaffoldeth.io/components/): Коллекция основных фронтенд компонентов для взаимодействия с Web3.  
- 🔥 **Burner Wallet & Local Faucet**: Тестируйте свои приложения с локальным источником криптовалюты. 
- 🔐 **Интеграция с провайдерами Web3**: Подключение основных провайдеров для доступа к сети Ethereum. 


![Debug Contracts tab](https://github.com/scaffold-eth/scaffold-eth-2/assets/55535804/1171422a-0ce4-4203-bcd4-d2d1941d198b)

## Requirements

- [Node (v18 LTS)](https://nodejs.org/en/download/)
- Yarn ([v1](https://classic.yarnpkg.com/en/docs/install/) or [v2+](https://yarnpkg.com/getting-started/install))
- [Git](https://git-scm.com/downloads)

## Начало работы

Для создания шаблонного приложения Scaffold-ETH 2, выполните следующие шаги:

1. Клонируйте репозиторий и установите зависимости

```
git clone https://github.com/labintsev/scaffold-eth-2-app.git
cd scaffold-eth-2-app
yarn install
```

2. В первом терминале запустите локальную Web3 сеть 

```
yarn chain
```
Эта команда запускает сеть Ethereum на локальной машине с помощью Hardhat для быстрой разработки и тестирования. 
Настройка параметров сети доступна в файле `hardhat.config.ts`.

3. Во втором терминале разместите и протестируйте смарт-контракт:

```
yarn deploy
```

Исходный код контракта расположен в папке `packages/hardhat/contracts`, его можно модифицировать для своего приложения. 
Команда `yarn deploy` размещает смарт-контракт в локальной сети, в папке `packages/hardhat/deploy`.
Скрипт для деплоя тоже можно кастомизировать. 

4. В третьем терминале запустите фронтенд-приложение NextJS:

```
yarn start
```

Перейдите по ссылке: `http://localhost:3000`. 
Взаимодействие со смарт-контрактом доступно на странице `Debug Contracts`. 
Настройки приложения доступны в файле `packages/nextjs/scaffold.config.ts`.

## Тестирование 

Запуск тестов для смарт-контракта командой `yarn hardhat:test`
Рекомендуется запускать тесты после каждого изменения
- исходного кода смарт-контракта `YourContract.sol` in `packages/hardhat/contracts`
- компонентов фронтенда `packages/nextjs/pages`
- настроек размещения скрипта в папке `packages/hardhat/deploy`

## Документация

Для подробного изучения компонентов Scaffold-ETH-2 обязательно посетите страницы [documentations](https://docs.scaffoldeth.io) и [website](https://scaffoldeth.io).

## Contributing to Scaffold-ETH 2

We welcome contributions to Scaffold-ETH 2!

Please see [CONTRIBUTING.MD](https://github.com/scaffold-eth/scaffold-eth-2/blob/main/CONTRIBUTING.md) for more information and guidelines for contributing to Scaffold-ETH 2.
