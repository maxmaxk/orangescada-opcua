# OrangeScada OPCUA driver

## Установка

Для работы использовать версию [Node.js](https://nodejs.org/) v16+

Для установки использовать команды

```sh
git clone https://github.com/maxmaxk/orangescada-opcua
cd orangescada-opcua
npm i
npm start
```
## Подключение к OrangeScada

Если использовать стандартный конфиг драйвера, то со стороны OrangeScada должен быть настроена работа с универсальным драйвером:
- порт: 8892
- ssl: выключено
- идентификатор драйвера: 1234
- пароль: password

## Тестирование

В тестовой конфигурации сервера прописано подключение к OPC-серверу от комании Prosys.
Для тестования необходимо инсталлировать [симулятор](https://downloads.prosysopc.com/opc-ua-simulation-server-downloads.php)

## Запуск драйвера как службы (для Windows)

Необходимо в папке драйвера выполнить команду

```sh
npm run installService
```

При удачном исполнении в списке служб появится `OrangeScadaOPCUADriver`, управляя которой можно запускать/останавливать универсальный драйвер

## License

MIT

