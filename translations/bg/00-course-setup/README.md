<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "c55b973b1562abf5aadf6a4028265ac5",
  "translation_date": "2025-08-29T21:05:40+00:00",
  "source_file": "00-course-setup/README.md",
  "language_code": "bg"
}
-->
# Настройка на курса

## Въведение

Този урок ще обхване как да стартирате примерите с код от този курс.

## Присъединете се към други обучаващи се и получете помощ

Преди да клонирате своето хранилище, се присъединете към [AI Agents For Beginners Discord канала](https://aka.ms/ai-agents/discord), за да получите помощ с настройката, да зададете въпроси относно курса или да се свържете с други обучаващи се.

## Клонирайте или форкнете това хранилище

За да започнете, клонирайте или форкнете GitHub хранилището. Това ще създаде ваша собствена версия на материалите от курса, така че да можете да стартирате, тествате и модифицирате кода!

Това може да се направи, като кликнете на линка към

Вече трябва да имате своя собствена форкната версия на този курс на следния линк:

![Forked Repo](../../../translated_images/forked-repo.33f27ca1901baa6a5e13ec3eb1f0ddd3a44d936d91cc8cfb19bfdb9688bd2c3d.bg.png)

## Стартиране на кода

Този курс предлага серия от Jupyter Notebooks, които можете да стартирате, за да получите практически опит в създаването на AI агенти.

Примерите с код използват следното:

**Изисква GitHub акаунт - Безплатно**:

1) Semantic Kernel Agent Framework + GitHub Models Marketplace. Обозначено като (semantic-kernel.ipynb)
2) AutoGen Framework + GitHub Models Marketplace. Обозначено като (autogen.ipynb)

**Изисква Azure абонамент**:
3) Azure AI Foundry + Azure AI Agent Service. Обозначено като (azureaiagent.ipynb)

Насърчаваме ви да изпробвате и трите типа примери, за да видите кой работи най-добре за вас.

Изборът ви ще определи кои стъпки за настройка трябва да следвате по-долу:

## Изисквания

- Python 3.12+
  - **NOTE**: Ако нямате инсталиран Python 3.12, уверете се, че го инсталирате. След това създайте своя venv, използвайки python3.12, за да гарантирате, че правилните версии са инсталирани от файла requirements.txt.
- GitHub акаунт - За достъп до GitHub Models Marketplace
- Azure абонамент - За достъп до Azure AI Foundry
- Azure AI Foundry акаунт - За достъп до Azure AI Agent Service

В корена на това хранилище сме включили файл `requirements.txt`, който съдържа всички необходими Python пакети за стартиране на примерите с код.

Можете да ги инсталирате, като изпълните следната команда в терминала в корена на хранилището:

```bash
pip install -r requirements.txt
```
Препоръчваме да създадете Python виртуална среда, за да избегнете конфликти и проблеми.

## Настройка на VSCode
Уверете се, че използвате правилната версия на Python в VSCode.

![image](https://github.com/user-attachments/assets/a85e776c-2edb-4331-ae5b-6bfdfb98ee0e)

## Настройка за примери с използване на GitHub модели

### Стъпка 1: Извличане на вашия GitHub Personal Access Token (PAT)

Този курс използва GitHub Models Marketplace, предоставяйки безплатен достъп до големи езикови модели (LLMs), които ще използвате за създаване на AI агенти.

За да използвате GitHub моделите, ще трябва да създадете [GitHub Personal Access Token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens).

Това може да се направи, като отидете на вашия GitHub акаунт.

Моля, следвайте [Принципа на минималните привилегии](https://docs.github.com/en/get-started/learning-to-code/storing-your-secrets-safely), когато създавате своя токен. Това означава, че трябва да дадете на токена само необходимите разрешения за стартиране на примерите с код от този курс.

1. Изберете опцията `Fine-grained tokens` от лявата страна на екрана, като отидете в **Developer settings**.
   ![](../../../translated_images/profile_developer_settings.410a859fe749c755c859d414294c5908e307222b2c61819c3203bbeed4470e25.bg.png)

    След това изберете `Generate new token`.

    ![Generate Token](../../../translated_images/fga_new_token.1c1a234afe202ab37483944a291ee80c1868e1e78082fd6bd4180fea5d5a15b4.bg.png)

2. Въведете описателно име за вашия токен, което отразява неговата цел, за да бъде лесно разпознаваем по-късно.

    🔐 Препоръка за продължителност на токена

    Препоръчителна продължителност: 30 дни  
    За по-сигурна настройка можете да изберете по-кратък период, например 7 дни 🛡️  
    Това е чудесен начин да си поставите лична цел и да завършите курса, докато мотивацията ви за учене е висока 🚀.

    ![Token Name and Expiration](../../../translated_images/token-name-expiry-date.a095fb0de63868640a4c82d6b1bbc92b482930a663917a5983a3c7cd1ef86b77.bg.png)

3. Ограничете обхвата на токена до вашия форк на това хранилище.

    ![Limit scope to fork repository](../../../translated_images/token_repository_limit.924ade5e11d9d8bb6cd21293987e4579dea860e2ba66d607fb46e49524d53644.bg.png)

4. Ограничете разрешенията на токена: Под **Permissions**, кликнете върху таба **Account** и натиснете бутона "+ Add permissions". Ще се появи падащо меню. Потърсете **Models** и поставете отметка.

    ![Add Models Permission](../../../translated_images/add_models_permissions.c0c44ed8b40fc143dc87792da9097d715b7de938354e8f771d65416ecc7816b8.bg.png)

5. Проверете изискваните разрешения, преди да генерирате токена.  
   ![Verify Permissions](../../../translated_images/verify_permissions.06bd9e43987a8b219f171bbcf519e45ababae35b844f5e9757e10afcb619b936.bg.png)

6. Преди да генерирате токена, уверете се, че сте готови да го съхраните на сигурно място, като например мениджър за пароли, тъй като той няма да бъде показан отново след създаването му.  
   ![Store Token Securely](../../../translated_images/store_token_securely.08ee2274c6ad6caf3482f1cd1bad7ca3fdca1ce737bc485bfa6499c84297c789.bg.png)

Копирайте новия токен, който току-що създадохте. Сега ще го добавите към файла `.env`, включен в този курс.

### Стъпка 2: Създайте вашия `.env` файл

За да създадете вашия `.env` файл, изпълнете следната команда в терминала.

```bash
cp .env.example .env
```

Това ще копира примерния файл и ще създаде `.env` във вашата директория, където ще попълните стойностите за променливите на средата.

С копирания токен отворете `.env` файла в любимия си текстов редактор и го поставете в полето `GITHUB_TOKEN`.  
![GitHub Token Field](../../../translated_images/github_token_field.20491ed3224b5f4ab24d10ced7a68c4aba2948fe8999cfc8675edaa16f5e5681.bg.png)

Сега трябва да можете да стартирате примерите с код от този курс.

## Настройка за примери с използване на Azure AI Foundry и Azure AI Agent Service

### Стъпка 1: Извличане на вашия Azure Project Endpoint

Следвайте стъпките за създаване на хъб и проект в Azure AI Foundry, описани тук: [Hub resources overview](https://learn.microsoft.com/en-us/azure/ai-foundry/concepts/ai-resources)

След като създадете своя проект, ще трябва да извлечете връзката за вашия проект.

Това може да се направи, като отидете на страницата **Overview** на вашия проект в Azure AI Foundry портала.

![Project Connection String](../../../translated_images/project-endpoint.8cf04c9975bbfbf18f6447a599550edb052e52264fb7124d04a12e6175e330a5.bg.png)

### Стъпка 2: Създайте вашия `.env` файл

За да създадете вашия `.env` файл, изпълнете следната команда в терминала.

```bash
cp .env.example .env
```

Това ще копира примерния файл и ще създаде `.env` във вашата директория, където ще попълните стойностите за променливите на средата.

С копирания токен отворете `.env` файла в любимия си текстов редактор и го поставете в полето `PROJECT_ENDPOINT`.

### Стъпка 3: Вход в Azure

Като най-добра практика за сигурност ще използваме [автентикация без ключ](https://learn.microsoft.com/azure/developer/ai/keyless-connections?tabs=csharp%2Cazure-cli?WT.mc_id=academic-105485-koreyst), за да се автентикираме към Azure OpenAI с Microsoft Entra ID.

След това отворете терминал и изпълнете `az login --use-device-code`, за да влезете във вашия Azure акаунт.

След като влезете, изберете вашия абонамент в терминала.

## Допълнителни променливи на средата - Azure Search и Azure OpenAI

За урока Agentic RAG - Урок 5 - има примери, които използват Azure Search и Azure OpenAI.

Ако искате да стартирате тези примери, ще трябва да добавите следните променливи на средата към вашия `.env` файл:

### Страница Overview (Проект)

- `AZURE_SUBSCRIPTION_ID` - Проверете **Project details** на страницата **Overview** на вашия проект.

- `AZURE_AI_PROJECT_NAME` - Погледнете в горната част на страницата **Overview** на вашия проект.

- `AZURE_OPENAI_SERVICE` - Намерете това в таба **Included capabilities** за **Azure OpenAI Service** на страницата **Overview**.

### Център за управление

- `AZURE_OPENAI_RESOURCE_GROUP` - Отидете на **Project properties** на страницата **Overview** на **Management Center**.

- `GLOBAL_LLM_SERVICE` - Под **Connected resources**, намерете името на връзката за **Azure AI Services**. Ако не е изброено, проверете **Azure портала** под вашата ресурсна група за името на ресурса AI Services.

### Страница Models + Endpoints

- `AZURE_OPENAI_EMBEDDING_DEPLOYMENT_NAME` - Изберете вашия embedding модел (например `text-embedding-ada-002`) и отбележете **Deployment name** от детайлите на модела.

- `AZURE_OPENAI_CHAT_DEPLOYMENT_NAME` - Изберете вашия chat модел (например `gpt-4o-mini`) и отбележете **Deployment name** от детайлите на модела.

### Azure портал

- `AZURE_OPENAI_ENDPOINT` - Потърсете **Azure AI services**, кликнете върху него, след това отидете на **Resource Management**, **Keys and Endpoint**, превъртете надолу до "Azure OpenAI endpoints" и копирайте този, който казва "Language APIs".

- `AZURE_OPENAI_API_KEY` - От същия екран копирайте KEY 1 или KEY 2.

- `AZURE_SEARCH_SERVICE_ENDPOINT` - Намерете вашия **Azure AI Search** ресурс, кликнете върху него и вижте **Overview**.

- `AZURE_SEARCH_API_KEY` - След това отидете на **Settings** и след това **Keys**, за да копирате основния или вторичния администраторски ключ.

### Външна уеб страница

- `AZURE_OPENAI_API_VERSION` - Посетете страницата [API version lifecycle](https://learn.microsoft.com/en-us/azure/ai-services/openai/api-version-deprecation#latest-ga-api-release) под **Latest GA API release**.

### Настройка на автентикация без ключ

Вместо да кодирате вашите идентификационни данни, ще използваме връзка без ключ с Azure OpenAI. За да направим това, ще импортираме `DefaultAzureCredential` и по-късно ще извикаме функцията `DefaultAzureCredential`, за да получим идентификационните данни.

```python
from azure.identity import DefaultAzureCredential, InteractiveBrowserCredential
```

## Нуждаете се от помощ?

Ако имате проблеми с изпълнението на тази настройка, влезте в нашия

## Следващ урок

Сега сте готови да стартирате кода за този курс. Приятно учене за света на AI агентите!

[Въведение в AI агентите и техните приложения](../01-intro-to-ai-agents/README.md)

---

**Отказ от отговорност**:  
Този документ е преведен с помощта на AI услуга за превод [Co-op Translator](https://github.com/Azure/co-op-translator). Въпреки че се стремим към точност, моля, имайте предвид, че автоматизираните преводи може да съдържат грешки или неточности. Оригиналният документ на неговия роден език трябва да се счита за авторитетен източник. За критична информация се препоръчва професионален човешки превод. Не носим отговорност за недоразумения или погрешни интерпретации, произтичащи от използването на този превод.