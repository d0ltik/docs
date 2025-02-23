---
title: "Как создать подключение к BigQuery"
description: "Следуя данной инструкции, вы сможете создать подключение к BigQuery."
---

# Создание подключения к Google BigQuery

{% note info %}

Для создания подключения сервисному аккаунту в BigQuery должна быть выдана роль [BigQuery User](https://cloud.google.com/bigquery/docs/access-control#bigquery.user) на датасет.
Подключение не поддерживает работу с партиционированными таблицами.

{% endnote %}

Чтобы создать подключение к BigQuery:

1. Перейдите на [страницу создания нового подключения]({{ link-datalens-main }}/connections/new).
1. В разделе **Базы данных** выберите подключение **BigQuery**.
1. Укажите параметры подключения:

   * **ID проекта**. Укажите идентификатор вашего проекта в Google Cloud.
   * **Приватный ключ сервисного аккаунта**. Нажмите кнопку **Прикрепить файл** и загрузите файл с авторизованным ключом вашего сервисного аккаунта Google Cloud — это необходимо для аутентификации. Подробнее о том, как получить файл с ключом, см. в [документации Google]( https://cloud.google.com/iam/docs/keys-create-delete).
   * **Уровень доступа SQL запросов**. Позволяет использовать произвольный SQL-запрос для [формирования датасета](../../dataset/settings.md#sql-request-in-datatset).
   * **Время жизни кеша в секундах**. Укажите время жизни кеша или оставьте значение по умолчанию. Рекомендованное значение — 300 секунд (5 минут).

1. (опционально) Проверьте работоспособность подключения. Для этого нажмите кнопку **Проверить подключение**.
1. Нажмите кнопку **Создать подключение**.
1. Выберите [воркбук](../../workbooks-collections/index.md), в котором сохранится подключение, или создайте новый. Если вы пользуетесь старой навигацией по папкам, выберите папку для сохранения подключения. Нажмите кнопку **Создать**.
1. Укажите название подключения и нажмите кнопку **Создать**.