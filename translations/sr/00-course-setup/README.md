<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "c55b973b1562abf5aadf6a4028265ac5",
  "translation_date": "2025-08-29T22:50:23+00:00",
  "source_file": "00-course-setup/README.md",
  "language_code": "sr"
}
-->
# Подешавање курса

## Увод

Ова лекција ће обухватити како да покренете узорке кода овог курса.

## Придружите се другим учесницима и добијте помоћ

Пре него што почнете са клонирањем вашег репозиторијума, придружите се [AI Agents For Beginners Discord каналу](https://aka.ms/ai-agents/discord) да добијете помоћ око подешавања, поставите питања о курсу или се повежете са другим учесницима.

## Клонирајте или форкујте овај репозиторијум

Да бисте започели, клонирајте или форкујте GitHub репозиторијум. Ово ће направити вашу верзију материјала курса како бисте могли да покрећете, тестирате и прилагођавате код!

Ово можете урадити кликом на линк до

Требало би да сада имате своју форковану верзију овог курса на следећем линку:

![Forked Repo](../../../translated_images/forked-repo.33f27ca1901baa6a5e13ec3eb1f0ddd3a44d936d91cc8cfb19bfdb9688bd2c3d.sr.png)

## Покретање кода

Овај курс нуди серију Jupyter Notebook-ова које можете покренути како бисте стекли практично искуство у изградњи AI агената.

Узорци кода користе:

**Захтева GitHub налог - бесплатно**:

1) Semantic Kernel Agent Framework + GitHub Models Marketplace. Ознака: (semantic-kernel.ipynb)
2) AutoGen Framework + GitHub Models Marketplace. Ознака: (autogen.ipynb)

**Захтева Azure претплату**:
3) Azure AI Foundry + Azure AI Agent Service. Ознака: (azureaiagent.ipynb)

Препоручујемо вам да испробате све три врсте примера како бисте видели који вам најбоље одговара.

Опција коју изаберете одредиће које кораке за подешавање треба да следите у наставку:

## Захтеви

- Python 3.12+
  - **НАПОМЕНА**: Ако немате Python 3.12 инсталиран, уверите се да сте га инсталирали. Затим креирајте свој venv користећи python3.12 како бисте осигурали да су исправне верзије инсталиране из датотеке requirements.txt.
- GitHub налог - за приступ GitHub Models Marketplace-у
- Azure претплата - за приступ Azure AI Foundry-у
- Azure AI Foundry налог - за приступ Azure AI Agent Service-у

У корену овог репозиторијума укључили смо датотеку `requirements.txt` која садржи све потребне Python пакете за покретање узорака кода.

Можете их инсталирати покретањем следеће команде у вашем терминалу у корену репозиторијума:

```bash
pip install -r requirements.txt
```
Препоручујемо креирање Python виртуелног окружења како бисте избегли било какве конфликте и проблеме.

## Подешавање VSCode-а
Уверите се да користите исправну верзију Python-а у VSCode-у.

![image](https://github.com/user-attachments/assets/a85e776c-2edb-4331-ae5b-6bfdfb98ee0e)

## Подешавање за узорке који користе GitHub моделе

### Корак 1: Преузмите свој GitHub Personal Access Token (PAT)

Овај курс користи GitHub Models Marketplace, који пружа бесплатан приступ великим језичким моделима (LLMs) које ћете користити за изградњу AI агената.

Да бисте користили GitHub моделе, потребно је да креирате [GitHub Personal Access Token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens).

Ово можете урадити тако што ћете отићи на свој

GitHub налог.

Молимо вас да следите [Принцип најмање привилегије](https://docs.github.com/en/get-started/learning-to-code/storing-your-secrets-safely) приликом креирања вашег токена. То значи да треба да доделите токену само оне дозволе које су му потребне за покретање узорака кода у овом курсу.

1. Изаберите опцију `Fine-grained tokens` на левој страни екрана тако што ћете отићи на **Developer settings**
   ![](../../../translated_images/profile_developer_settings.410a859fe749c755c859d414294c5908e307222b2c61819c3203bbeed4470e25.sr.png)

    Затим изаберите `Generate new token`.

    ![Generate Token](../../../translated_images/fga_new_token.1c1a234afe202ab37483944a291ee80c1868e1e78082fd6bd4180fea5d5a15b4.sr.png)

2. Унесите описно име за ваш токен које одражава његову сврху, чинећи га лако препознатљивим касније.

    🔐 Препорука за трајање токена

    Препоручено трајање: 30 дана  
    За сигурнији приступ можете изабрати краћи период—на пример, 7 дана 🛡️  
    То је одличан начин да поставите лични циљ и завршите курс док је ваш ентузијазам за учење висок 🚀.

    ![Token Name and Expiration](../../../translated_images/token-name-expiry-date.a095fb0de63868640a4c82d6b1bbc92b482930a663917a5983a3c7cd1ef86b77.sr.png)

3. Ограничите опсег токена на ваш форк овог репозиторијума.

    ![Limit scope to fork repository](../../../translated_images/token_repository_limit.924ade5e11d9d8bb6cd21293987e4579dea860e2ba66d607fb46e49524d53644.sr.png)

4. Ограничите дозволе токена: Под **Permissions**, кликните на картицу **Account**, а затим на дугме "+ Add permissions". Појавиће се падајући мени. Потражите **Models** и означите поље за њега.
    ![Add Models Permission](../../../translated_images/add_models_permissions.c0c44ed8b40fc143dc87792da9097d715b7de938354e8f771d65416ecc7816b8.sr.png)

5. Потврдите потребне дозволе пре него што генеришете токен. ![Verify Permissions](../../../translated_images/verify_permissions.06bd9e43987a8b219f171bbcf519e45ababae35b844f5e9757e10afcb619b936.sr.png)

6. Пре него што генеришете токен, уверите се да сте спремни да га сачувате на сигурном месту, као што је менаџер лозинки, јер неће бити приказан поново након креирања. ![Store Token Securely](../../../translated_images/store_token_securely.08ee2274c6ad6caf3482f1cd1bad7ca3fdca1ce737bc485bfa6499c84297c789.sr.png)

Копирајте свој нови токен који сте управо креирали. Сада ћете га додати у вашу `.env` датотеку укључену у овај курс.

### Корак 2: Креирајте своју `.env` датотеку

Да бисте креирали `.env` датотеку, покрените следећу команду у вашем терминалу.

```bash
cp .env.example .env
```

Ово ће копирати пример датотеке и креирати `.env` у вашем директоријуму где ћете попунити вредности за променљиве окружења.

Са копираним токеном, отворите `.env` датотеку у вашем омиљеном текст едитору и налепите ваш токен у поље `GITHUB_TOKEN`.  
![GitHub Token Field](../../../translated_images/github_token_field.20491ed3224b5f4ab24d10ced7a68c4aba2948fe8999cfc8675edaa16f5e5681.sr.png)

Сада би требало да можете да покренете узорке кода овог курса.

## Подешавање за узорке који користе Azure AI Foundry и Azure AI Agent Service

### Корак 1: Преузмите свој Azure Project Endpoint

Пратите кораке за креирање хаба и пројекта у Azure AI Foundry-у овде: [Hub resources overview](https://learn.microsoft.com/en-us/azure/ai-foundry/concepts/ai-resources)

Када креирате свој пројекат, потребно је да преузмете стринг за повезивање вашег пројекта.

Ово можете урадити тако што ћете отићи на страницу **Overview** вашег пројекта у Azure AI Foundry порталу.

![Project Connection String](../../../translated_images/project-endpoint.8cf04c9975bbfbf18f6447a599550edb052e52264fb7124d04a12e6175e330a5.sr.png)

### Корак 2: Креирајте своју `.env` датотеку

Да бисте креирали `.env` датотеку, покрените следећу команду у вашем терминалу.

```bash
cp .env.example .env
```

Ово ће копирати пример датотеке и креирати `.env` у вашем директоријуму где ћете попунити вредности за променљиве окружења.

Са копираним токеном, отворите `.env` датотеку у вашем омиљеном текст едитору и налепите ваш токен у поље `PROJECT_ENDPOINT`.

### Корак 3: Пријавите се на Azure

Као најбољу праксу за безбедност, користићемо [аутентификацију без кључа](https://learn.microsoft.com/azure/developer/ai/keyless-connections?tabs=csharp%2Cazure-cli?WT.mc_id=academic-105485-koreyst) за аутентификацију на Azure OpenAI са Microsoft Entra ID.

Затим, отворите терминал и покрените `az login --use-device-code` да се пријавите на ваш Azure налог.

Када се пријавите, изаберите вашу претплату у терминалу.

## Додатне променљиве окружења - Azure Search и Azure OpenAI

За лекцију Agentic RAG - Лекција 5 - постоје узорци који користе Azure Search и Azure OpenAI.

Ако желите да покренете ове узорке, потребно је да додате следеће променљиве окружења у вашу `.env` датотеку:

### Страница прегледа (Пројекат)

- `AZURE_SUBSCRIPTION_ID` - Проверите **Project details** на страници **Overview** вашег пројекта.

- `AZURE_AI_PROJECT_NAME` - Погледајте врх странице **Overview** вашег пројекта.

- `AZURE_OPENAI_SERVICE` - Пронађите ово у картици **Included capabilities** за **Azure OpenAI Service** на страници **Overview**.

### Центар за управљање

- `AZURE_OPENAI_RESOURCE_GROUP` - Идите на **Project properties** на страници **Overview** у **Management Center**.

- `GLOBAL_LLM_SERVICE` - Под **Connected resources**, пронађите име везе за **Azure AI Services**. Ако није наведено, проверите **Azure portal** у вашој групи ресурса за име ресурса AI Services.

### Страница модела + крајњих тачака

- `AZURE_OPENAI_EMBEDDING_DEPLOYMENT_NAME` - Изаберите свој модел за уграђивање (нпр. `text-embedding-ada-002`) и забележите **Deployment name** из детаља модела.

- `AZURE_OPENAI_CHAT_DEPLOYMENT_NAME` - Изаберите свој модел за ћаскање (нпр. `gpt-4o-mini`) и забележите **Deployment name** из детаља модела.

### Azure портал

- `AZURE_OPENAI_ENDPOINT` - Потражите **Azure AI services**, кликните на њега, затим идите на **Resource Management**, **Keys and Endpoint**, скролујте до "Azure OpenAI endpoints" и копирајте онај који каже "Language APIs".

- `AZURE_OPENAI_API_KEY` - Са истог екрана, копирајте КЉУЧ 1 или КЉУЧ 2.

- `AZURE_SEARCH_SERVICE_ENDPOINT` - Пронађите свој **Azure AI Search** ресурс, кликните на њега и погледајте **Overview**.

- `AZURE_SEARCH_API_KEY` - Затим идите на **Settings** и затим **Keys** да копирате примарни или секундарни администраторски кључ.

### Спољна веб страница

- `AZURE_OPENAI_API_VERSION` - Посетите страницу [API version lifecycle](https://learn.microsoft.com/en-us/azure/ai-services/openai/api-version-deprecation#latest-ga-api-release) под **Latest GA API release**.

### Подешавање аутентификације без кључа

Уместо да хардкодујете своје акредитиве, користићемо везу без кључа са Azure OpenAI. Да бисмо то урадили, увешћемо `DefaultAzureCredential` и касније позвати функцију `DefaultAzureCredential` да добијемо акредитиве.

```python
from azure.identity import DefaultAzureCredential, InteractiveBrowserCredential
```

## Заглавили сте негде?

Ако имате било каквих проблема са покретањем овог подешавања, придружите се нашем

или.

## Следећа лекција

Сада сте спремни да покренете код за овај курс. Срећно у учењу више о свету AI агената!

[Увод у AI агенте и њихове случајеве употребе](../01-intro-to-ai-agents/README.md)

---

**Одрицање од одговорности**:  
Овај документ је преведен коришћењем услуге за превођење помоћу вештачке интелигенције [Co-op Translator](https://github.com/Azure/co-op-translator). Иако се трудимо да обезбедимо тачност, молимо вас да имате у виду да аутоматски преводи могу садржати грешке или нетачности. Оригинални документ на његовом изворном језику треба сматрати меродавним извором. За критичне информације препоручује се професионални превод од стране људи. Не преузимамо одговорност за било каква погрешна тумачења или неспоразуме који могу настати услед коришћења овог превода.