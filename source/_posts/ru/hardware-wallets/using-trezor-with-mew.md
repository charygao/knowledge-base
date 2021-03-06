---
title: "Использование аппаратного кошелька Trezor с MEW"
date: 2018-06-01 00:01:00
tags:
  - trezor
  - аппаратный
  - кошелек
categories:
  - 
    - аппаратные-кошельки
primary_category: аппаратные-кошельки
primary_category_display_name: "Аппаратные кошельки"
alias:
  - migration/moving-from-private-key-to-trezor-hardware-wallet.html
---

# **Использование аппаратного кошелька Trezor с MEW**

###### {% read_time title "Использование аппаратного кошелька Trezor с MEW" %} мин. на прочтение

* * *

Аппаратные кошельки Trezor являются одними из самых безопасных и простых в использовании аппаратных кошельков для криптовалют. Если у вас нет такого кошелька, его можно приобрести [через веб-сайт компании](https://trezor.io/?offer_id=12&aff_id=2029).

_Пожалуйста, приобретайте аппаратные кошельки в официальном магазине. На аппаратные кошельки, купленные на Ebay или у других поставщиков, не распространяются гарантии безопасности._

Данный аппаратный кошелек поддерживает широкий спектр криптовалют, но это руководство было специально разработано для описания работы с токенам Ethereum и ERC-20 с использованием MyEtherWallet (MEW).

**Этот пункт очень важен.** Ваше устройство Trezor является ОТДЕЛЬНЫМ кошельком. Вы не сможете импортировать свой старый адрес MEW или использовать старый кошелек с устройством. Кошелек обладает собственным закрытым ключом, зашифрованным в самом устройстве. Вам нужно будет выбрать новый адрес ethereum для использования с устройством и пользоваться им как новым основным кошельком.

Ну что ж, давайте начнем!

## **Начальная настройка**

**Шаг 1.** Распакуйте ваш Trezor! Вы увидите несколько карт и инструкций для настройки. Внимательно следуйте этим инструкциям! Подключите Trezor к своему компьютеру и начните работу с ним. Перейдите на [trezor.io/start](https://trezor.io/start), чтобы начать процесс настройки.

<img src="/images/posts/hardware-wallet/trezor/Trezor1.jpg" width="35%" />

* * *

**Шаг 2.** Выберите "Создать новый" на этой странице и выполните все необходимые действия для настройки вашего нового устройства. Первое, что стоит сделать, — "Создать резервную копию за 3 минуты".

<img src="/images/posts/hardware-wallet/trezor/Trezor2.png" width="80%" />

* * *

**Шаг 3.** _Это один из самых важных шагов._ Не записывайте эту фразу на вашем компьютере, не делайте фото фразы. Запишите свои 24 seed-слова в нескольких местах. НЕ ПОТЕРЯЙТЕ ИХ. Если вы потеряете эти слова, вы потеряете также и доступ ко всей своей криптовалюте. В комплекте с Ledger поставляются карточки для записи, но я предлагаю записать их еще где-нибудь. И еще раз, не сохраняйте эту фразу на своем компьютере. Используйте ручку и бумагу. Когда вы закончите, то увидите экран приведенный ниже.

<img src="/images/posts/hardware-wallet/trezor/Trezor3.png" width="80%" />

<img src="/images/posts/hardware-wallet/trezor/Trezor4.png" width="75%" />

* * *

**Шаг 4.** Теперь вам предложат выбрать имя для вашего устройства Trezor. Его вы будете видеть на своем устройстве при каждом подключении. Выберите что-нибудь знакомое и лично ваше!

<img src="/images/posts/hardware-wallet/trezor/Trezor5.png" width="70%" />

<img src="/images/posts/hardware-wallet/trezor/Trezor6.png" width="75%" />

* * *

**Шаг 5.** Теперь необходимо выбрать PIN-код. Он станет единственным способом получения доступа к вашему устройству (помимо фразы восстановления, которую вы уже записали несколько раз), поэтому очень важно выбрать безопасный, но легко запоминающийся пин-код. Не используйте комбинации `1111` или `1234`, выберите что-то более случайное и безопасное. _Не допускайте эту ошибку! Если вы получите сообщение, что код может быть безопаснее, сделайте его длиннее!_

<img src="/images/posts/hardware-wallet/trezor/Trezor7.png" width="75%" />

<img src="/images/posts/hardware-wallet/trezor/Trezor8.png" width="70%" />

* * *

**Шаг 6.** Все готово!

<img src="/images/posts/hardware-wallet/trezor/Trezor9.png" width="50%" />

## **Использование Trezor с MEW**

**Шаг 1.** Подключите ваше устройство Trezor и направляйтесь на сайт MEW.

<img src="/images/posts/hardware-wallet/trezor/Trezor10.jpg" width="35%" />

* * *

**Шаг 2.** Проверьте URL-адрес SSL сертификата MyEtherWallet Inc [US], чтобы убедиться, что вы на нашем настоящем и безопасном сайте. Вы уверены? Отлично! Перейдите на ‘Доступ к кошельку’ и выберите пункт ‘Аппаратные кошельки’. Выберите ‘Trezor’ и ‘Продолжить’. В это время Trezor все еще должен быть подключен.

<img src="/images/posts/hardware-wallet/trezor/MEW1.png" width="75%" />

* * *

**Шаг 3.** Появится всплывающее окно с запросом на предоставление разрешений MEW на чтение публичных ключей с вашего устройства Trezor. Нажмите ‘Allow once for this session’ и выберите опцию ‘Don’t ask me again’, чтобы пропускать этот шаг в будущем. Нажмите ‘Export’ на следующем экране и введите свой пин-код, после чего вас перенаправит обратно на MEW.

<img src="/images/posts/hardware-wallet/trezor/MEW2.png" width="70%" />

<img src="/images/posts/hardware-wallet/trezor/Trezor11.png" width="70%" />

* * *

**Шаг 4.** MEW вернет вас на страницу с разными сетями и путями деривации. Выберите сеть, к которой хотите подключиться, и путь деривации. Для использования обычного ETH вы должны быть в сети ETH с путем деривации Ethereum. Вы также можете получить доступ к другим сетям, таким как Ethereum Classic (ETC), выбрав соответствующую опцию.

<img src="/images/posts/hardware-wallet/trezor/Trezor16.png" width="40%" /> <img src="/images/posts/hardware-wallet/trezor/Trezor12.png" width="40%" />

<img src="/images/posts/hardware-wallet/trezor/Trezor17.png" width="40%" />

* * *

**Шаг 5.** Вы увидите список адресов. Это новые адреса, доступные для выбора в качестве вашего основного кошелька! Выберите один из пяти, который вам нравится. (Большинство людей выбирают первый, но это не обязательно.)

<img src="/images/posts/hardware-wallet/trezor/Trezor13.png" width="42.5%" /> <img src="/images/posts/hardware-wallet/trezor/Trezor14.png" width="50%" />

* * *

**Шаг 6.** Теперь вас должны перенаправить в окно, очень похожее на окно доступа к вашему старому кошельку. Отличная работа! Теперь вы официально используете свой новый аппаратный кошелек Trezor!

<img src="/images/posts/hardware-wallet/trezor/Trezor15.png" width="50%" />

## **А что насчет моего старого кошелька???**

Если вы переходите со старого кошелька и хотите, чтобы ваши ETH и токены были доступны на новом безопасном адресе Trezor, вам нужно будет перевести средства на новый адрес через обычную транзакцию. Это можно сделать, войдя в ваш старый кошелек с помощью MEW wallet, MetaMask, файла хранилища ключей или закрытого ключа (как вы обычно делали это до перехода на Trezor). Переведите свои ETH и токены на новый адрес Trezor с более безопасным доступом.

Обращаем ваше внимание, что для перевода токенов со старого кошелька потребуется оплата комиссии газа в ETH. Мы рекомендуем иметь 0.01 ETH, которых хватит для совершения 2—3 транзакций.

## **Как мне восстановить доступ к Trezor на новом устройстве?**

У Trezor есть [понятное и простое руководство](https://wiki.trezor.io/User_manual:Recovery) о том, как восстановить ваше устройство.

## **Решение проблем**

Большинство проблем с Trezor можно решить, выполнив принудительное обновление страницы (с помощью сочетания клавиш CTRL+F5), использования последней версии прошивки, а также нового кабеля для подключения.

Как всегда, не стесняйтесь связаться с нами по адресу [support@myetherwallet.com.](mailto:support@myetherwallet.com.) Мы всегда рады помочь!
