---
title: "Создать Multi-Collateral Vault с MakerDAO"
date: 2018-06-01 00:02:00
tags:
  - makerdao
  - defi
  - cdp
  - dai
  - mkr
  - dapps
categories:
  - 
    - dapps
primary_category: dapps
primary_category_display_name: "Dapps"
---

# **Создать Multi-Collateral Vault с MakerDAO**

###### {% read_time title "Open a Multi-Collateral Vault with MakerDAO" %} минут на чтение

* * *

###### Если вы хотите открыть Vault с помощью нашего приложения MakerDAO Dapp, вам понадобится кошелек для [доступа к нашему интерфейсу](/@@@@@@/getting-started/how-to-access-your-wallet/). Если у вас нет кошелька, [ нажмите сюда](/@@@@@@/getting-started/how-to-create-a-wallet/), чтобы его создать.

## **Создание Vault**

**Шаг 1.** Откройте ваш кошелек на нашем сайте, выбрав "Доступ к кошельку", а затем способ доступа.

<img src="/images/posts/diving-deeper/ENS1-1.png
" alt="Image of MEW main page" width="100%" />

**Шаг 2.** Направляйтесь в наш раздел Dapps в левой части страницы "Обзор кошелька", а затем выберите MakerDAO.

<img src="/images/posts/diving-deeper/MKR1.png" alt="Image of MakerDAO in Dapps page" width="100%" />

**Шаг 3.** Для начала выберите «Создать Vault».

-   Если вы создавали CDP в прошлом, вам нужно будет выполнить процедуры описанные в разделах "Обновить 'старый' DA на 'новый' DAI" и "Миграция CDP однотипного залога в Vault разнотипного залога".

<img src="/images/posts/diving-deeper/MKR2.png" alt="Image of MakerDAO main page" width="100%" />

**Шаг 4.** Укажите сумму ETH, которую вы хотите предложить в качестве залога. Не забудьте оставить небольшой зазор чтобы учитывать изменения на рынках. Как правило, 200% и выше – это безопасный вариант.

-   Перед тем как сгенерировать ваше хранилище, вам нужно выбрать 'Создать прокси'.
-   Подтвердите транзакции на вашем устройстве, если вы его используете.

<img src="/images/posts/diving-deeper/MKR3.png" alt="Image of offering collateral to generate a vault " width="100%" />

<img src="/images/posts/diving-deeper/MKR4.png" alt="Image of confirming the MakerDAO transaction" width="80%" />

**Шаг 5.** Страница MakerDAO изменится и отобразит данные о ваших вкладах.

<img src="/images/posts/diving-deeper/MKR5.png" alt="Image of MakerDAO vault overview page" width="100%" />

## **Зарабатывайте проценты с помощью DAI**

**Шаг 1.** Перейдите на страницу MakerDAO Dapp и выберите 'Сбережения DAI'.

<img src="/images/posts/diving-deeper/MKR2.png" alt="Image of MakerDAO main page" width="100%" />

**Шаг 2.** Выберите 'Установить', чтобы установить разрешение Maker для взаимодействия с вашим DAI.

-   Если вы взаимодействуете с Maker в первый раз, вам надо будет применить прокси. Выберете "Установка" в верхней части этого раздела.

<img src="/images/posts/diving-deeper/MKR6.png" alt="Image of 'Set Allowance'" width="80%" />

**Шаг 3.** Выберите, сколько DAI вы хотели бы внести в депозит. Процентные ставки начисляются ежегодно.

<img src="/images/posts/diving-deeper/MKR7.png" alt="Image of depositing DAI" width="80%" />

**Шаг 4.** Для снятия выполните ту же процедуру, но выберите «Вывести».

<img src="/images/posts/diving-deeper/MKR8.png" alt="Image of withdrawing DAI" width="80%" />

## **Закрытие Vault**

**Шаг 1.** Когда вы будете готовы, вернитесь в раздел Dapps и выберите MakerDAO.

<img src="/images/posts/diving-deeper/MKR1.png" alt="Image of MakerDAO main page" width="100%" />

**Шаг 2.** Нажмите «Управление Vault», чтобы увидеть ваши средства.

<img src="/images/posts/diving-deeper/MKR9.png" alt="Image of MakerDAO vault main page" width="100%" />

**Шаг 3.** Вам нужно будет вернуть DAI для вывода ETH. В разделе 'Позиция DAI' выберите 'Вернуть >'.

-   Вам потребуется "Утвердить" количество DAI прежде чем вернуть его. Это будет считаться отдельной транзакцией.
-   Пожалуйста, дождитесь чтобы обе транзакции имели статус "Успех", прежде чем продолжить.

<img src="/images/posts/diving-deeper/MKR10.png" alt="Image of DAI repayment" width="80%" />

<img src="/images/posts/diving-deeper/MKR11.png" alt="Image of updated vault details" width="100%" />

**Шаг 4.** После утверждения и оплаты DAI, вы можете снять ETH. Под «Залог ETH» выберите «Вывести >».

<img src="/images/posts/diving-deeper/MKR12.png" alt="Image of withdrawing collateral" width="80%" />

<img src="/images/posts/diving-deeper/MKR13.png" alt="Image of empty vault" width="100%" />

**Шаг 5.** На самом деле ваш Vault не _закрывается_, а остается пустым и готовым, если вам когда-нибудь нужно использовать его снова.

## **Вот видео, показывающее процесс:**

<div class="youtube-video">
<iframe width="560" height="315" src="https://www.youtube.com/embed/xNK_px6vPEM" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
