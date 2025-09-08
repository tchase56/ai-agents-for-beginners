<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "c55b973b1562abf5aadf6a4028265ac5",
  "translation_date": "2025-08-29T12:26:38+00:00",
  "source_file": "00-course-setup/README.md",
  "language_code": "ru"
}
-->
# Настройка курса

## Введение

В этом уроке мы рассмотрим, как запускать примеры кода из данного курса.

## Присоединяйтесь к другим учащимся и получайте помощь

Прежде чем клонировать репозиторий, присоединяйтесь к [каналу Discord "AI Agents For Beginners"](https://aka.ms/ai-agents/discord), чтобы получить помощь с настройкой, задать вопросы по курсу или пообщаться с другими учащимися.

## Клонируйте или форкните этот репозиторий

Для начала клонируйте или форкните репозиторий на GitHub. Это создаст вашу собственную версию материалов курса, чтобы вы могли запускать, тестировать и изменять код!

Это можно сделать, перейдя по ссылке:

![Forked Repo](../../../translated_images/forked-repo.33f27ca1901baa6a5e13ec3eb1f0ddd3a44d936d91cc8cfb19bfdb9688bd2c3d.ru.png)

## Запуск кода

Этот курс предлагает серию Jupyter Notebook, которые вы можете использовать для практического изучения создания AI-агентов.

Примеры кода используют следующие инструменты:

**Требуется аккаунт GitHub (бесплатно):**

1) Semantic Kernel Agent Framework + GitHub Models Marketplace. Обозначено как (semantic-kernel.ipynb)
2) AutoGen Framework + GitHub Models Marketplace. Обозначено как (autogen.ipynb)

**Требуется подписка Azure:**
3) Azure AI Foundry + Azure AI Agent Service. Обозначено как (azureaiagent.ipynb)

Мы рекомендуем попробовать все три типа примеров, чтобы понять, какой из них подходит вам лучше всего.

Выбранный вами вариант определит, какие шаги настройки нужно выполнить ниже:

## Требования

- Python 3.12+
  - **NOTE**: Если у вас не установлен Python 3.12, убедитесь, что вы его установили. Затем создайте виртуальное окружение (venv) с использованием python3.12, чтобы гарантировать установку правильных версий из файла requirements.txt.
- Аккаунт GitHub — для доступа к GitHub Models Marketplace
- Подписка Azure — для доступа к Azure AI Foundry
- Аккаунт Azure AI Foundry — для доступа к Azure AI Agent Service

Мы включили файл `requirements.txt` в корневую папку этого репозитория, который содержит все необходимые Python-библиотеки для запуска примеров кода.

Вы можете установить их, выполнив следующую команду в терминале в корневой папке репозитория:

```bash
pip install -r requirements.txt
```
Мы рекомендуем создать виртуальное окружение Python, чтобы избежать конфликтов и проблем.

## Настройка VSCode
Убедитесь, что вы используете правильную версию Python в VSCode.

![image](https://github.com/user-attachments/assets/a85e776c-2edb-4331-ae5b-6bfdfb98ee0e)

## Настройка для примеров с использованием GitHub Models 

### Шаг 1: Получите ваш персональный токен доступа (PAT) GitHub

Этот курс использует GitHub Models Marketplace, предоставляющий бесплатный доступ к большим языковым моделям (LLM), которые вы будете использовать для создания AI-агентов.

Чтобы использовать GitHub Models, вам нужно создать [персональный токен доступа GitHub](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens).

Это можно сделать, перейдя в ваш аккаунт GitHub.

Пожалуйста, следуйте [принципу минимальных привилегий](https://docs.github.com/en/get-started/learning-to-code/storing-your-secrets-safely) при создании токена. Это означает, что вы должны предоставить токену только те разрешения, которые необходимы для выполнения примеров кода из этого курса.

1. Выберите опцию `Fine-grained tokens` в левой части экрана, перейдя в **Developer settings**.
   ![](../../../translated_images/profile_developer_settings.410a859fe749c755c859d414294c5908e307222b2c61819c3203bbeed4470e25.ru.png)

    Затем выберите `Generate new token`.

    ![Generate Token](../../../translated_images/fga_new_token.1c1a234afe202ab37483944a291ee80c1868e1e78082fd6bd4180fea5d5a15b4.ru.png)

2. Введите описательное имя для вашего токена, чтобы позже было легко понять его назначение.

    🔐 Рекомендация по сроку действия токена

    Рекомендуемый срок действия: 30 дней.  
    Для большей безопасности вы можете выбрать более короткий срок, например, 7 дней 🛡️.  
    Это отличный способ поставить себе цель и завершить курс, пока ваш интерес к обучению высок 🚀.

    ![Token Name and Expiration](../../../translated_images/token-name-expiry-date.a095fb0de63868640a4c82d6b1bbc92b482930a663917a5983a3c7cd1ef86b77.ru.png)

3. Ограничьте область действия токена вашим форком этого репозитория.

    ![Limit scope to fork repository](../../../translated_images/token_repository_limit.924ade5e11d9d8bb6cd21293987e4579dea860e2ba66d607fb46e49524d53644.ru.png)

4. Ограничьте разрешения токена: в разделе **Permissions** выберите вкладку **Account** и нажмите кнопку "+ Add permissions". Появится выпадающее меню. Найдите **Models** и установите для него галочку.
    ![Add Models Permission](../../../translated_images/add_models_permissions.c0c44ed8b40fc143dc87792da9097d715b7de938354e8f771d65416ecc7816b8.ru.png)

5. Проверьте необходимые разрешения перед созданием токена. ![Verify Permissions](../../../translated_images/verify_permissions.06bd9e43987a8b219f171bbcf519e45ababae35b844f5e9757e10afcb619b936.ru.png)

6. Перед созданием токена убедитесь, что вы готовы сохранить его в безопасном месте, например, в хранилище паролей, так как он больше не будет отображаться после создания. ![Store Token Securely](../../../translated_images/store_token_securely.08ee2274c6ad6caf3482f1cd1bad7ca3fdca1ce737bc485bfa6499c84297c789.ru.png)

Скопируйте ваш новый токен. Теперь вы добавите его в файл `.env`, включенный в этот курс.

### Шаг 2: Создайте файл `.env`

Чтобы создать файл `.env`, выполните следующую команду в терминале:

```bash
cp .env.example .env
```

Эта команда скопирует пример файла и создаст `.env` в вашем каталоге, где вы заполните значения для переменных окружения.

Скопировав токен, откройте файл `.env` в вашем любимом текстовом редакторе и вставьте токен в поле `GITHUB_TOKEN`.
![GitHub Token Field](../../../translated_images/github_token_field.20491ed3224b5f4ab24d10ced7a68c4aba2948fe8999cfc8675edaa16f5e5681.ru.png)

Теперь вы должны быть готовы к запуску примеров кода из этого курса.

## Настройка для примеров с использованием Azure AI Foundry и Azure AI Agent Service

### Шаг 1: Получите конечную точку вашего проекта Azure

Следуйте инструкциям по созданию хаба и проекта в Azure AI Foundry, которые можно найти здесь: [Обзор ресурсов хаба](https://learn.microsoft.com/en-us/azure/ai-foundry/concepts/ai-resources).

После создания проекта вам нужно будет получить строку подключения для вашего проекта.

Это можно сделать на странице **Overview** вашего проекта в портале Azure AI Foundry.

![Project Connection String](../../../translated_images/project-endpoint.8cf04c9975bbfbf18f6447a599550edb052e52264fb7124d04a12e6175e330a5.ru.png)

### Шаг 2: Создайте файл `.env`

Чтобы создать файл `.env`, выполните следующую команду в терминале:

```bash
cp .env.example .env
```

Эта команда скопирует пример файла и создаст `.env` в вашем каталоге, где вы заполните значения для переменных окружения.

Скопировав токен, откройте файл `.env` в вашем любимом текстовом редакторе и вставьте токен в поле `PROJECT_ENDPOINT`.

### Шаг 3: Войдите в Azure

В качестве лучшей практики безопасности мы будем использовать [аутентификацию без ключей](https://learn.microsoft.com/azure/developer/ai/keyless-connections?tabs=csharp%2Cazure-cli?WT.mc_id=academic-105485-koreyst) для аутентификации в Azure OpenAI с помощью Microsoft Entra ID.

Откройте терминал и выполните команду `az login --use-device-code`, чтобы войти в ваш аккаунт Azure.

После входа выберите вашу подписку в терминале.

## Дополнительные переменные окружения — Azure Search и Azure OpenAI

Для урока Agentic RAG (Урок 5) есть примеры, использующие Azure Search и Azure OpenAI.

Если вы хотите запустить эти примеры, вам нужно будет добавить следующие переменные окружения в ваш файл `.env`:

### Страница Overview (Проект)

- `AZURE_SUBSCRIPTION_ID` — Проверьте **Project details** на странице **Overview** вашего проекта.

- `AZURE_AI_PROJECT_NAME` — Посмотрите в верхней части страницы **Overview** вашего проекта.

- `AZURE_OPENAI_SERVICE` — Найдите это на вкладке **Included capabilities** для **Azure OpenAI Service** на странице **Overview**.

### Центр управления

- `AZURE_OPENAI_RESOURCE_GROUP` — Перейдите в **Project properties** на странице **Overview** Центра управления.

- `GLOBAL_LLM_SERVICE` — В разделе **Connected resources** найдите имя подключения **Azure AI Services**. Если оно не указано, проверьте **Azure portal** в вашей группе ресурсов для имени ресурса AI Services.

### Страница Models + Endpoints

- `AZURE_OPENAI_EMBEDDING_DEPLOYMENT_NAME` — Выберите вашу модель встраивания (например, `text-embedding-ada-002`) и запишите **Deployment name** из деталей модели.

- `AZURE_OPENAI_CHAT_DEPLOYMENT_NAME` — Выберите вашу модель чата (например, `gpt-4o-mini`) и запишите **Deployment name** из деталей модели.

### Портал Azure

- `AZURE_OPENAI_ENDPOINT` — Найдите **Azure AI services**, нажмите на него, затем перейдите в **Resource Management**, **Keys and Endpoint**, прокрутите вниз до "Azure OpenAI endpoints" и скопируйте тот, который указан как "Language APIs".

- `AZURE_OPENAI_API_KEY` — На той же странице скопируйте KEY 1 или KEY 2.

- `AZURE_SEARCH_SERVICE_ENDPOINT` — Найдите ваш ресурс **Azure AI Search**, нажмите на него и посмотрите **Overview**.

- `AZURE_SEARCH_API_KEY` — Затем перейдите в **Settings**, затем **Keys**, чтобы скопировать основной или вторичный административный ключ.

### Внешняя страница

- `AZURE_OPENAI_API_VERSION` — Посетите страницу [API version lifecycle](https://learn.microsoft.com/en-us/azure/ai-services/openai/api-version-deprecation#latest-ga-api-release) в разделе **Latest GA API release**.

### Настройка аутентификации без ключей

Вместо жесткого кодирования ваших учетных данных мы будем использовать подключение без ключей с Azure OpenAI. Для этого мы импортируем `DefaultAzureCredential` и позже вызовем функцию `DefaultAzureCredential`, чтобы получить учетные данные.

```python
from azure.identity import DefaultAzureCredential, InteractiveBrowserCredential
```

## Застряли на каком-то этапе?

Если у вас возникли проблемы с настройкой, присоединяйтесь к нашему

## Следующий урок

Теперь вы готовы к запуску кода из этого курса. Удачного изучения мира AI-агентов!

[Введение в AI-агентов и их применение](../01-intro-to-ai-agents/README.md)

---

**Отказ от ответственности**:  
Этот документ был переведен с помощью сервиса автоматического перевода [Co-op Translator](https://github.com/Azure/co-op-translator). Несмотря на наши усилия по обеспечению точности, пожалуйста, учитывайте, что автоматические переводы могут содержать ошибки или неточности. Оригинальный документ на его родном языке следует считать авторитетным источником. Для получения критически важной информации рекомендуется профессиональный перевод человеком. Мы не несем ответственности за любые недоразумения или неправильные интерпретации, возникающие в результате использования данного перевода.