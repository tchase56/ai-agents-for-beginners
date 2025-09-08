<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "4a5ccc4ad1dba85fbc2087cf3b986544",
  "translation_date": "2025-08-29T23:43:06+00:00",
  "source_file": "04-tool-use/README.md",
  "language_code": "uk"
}
-->
[![Як створювати якісних AI-агентів](../../../translated_images/lesson-4-thumbnail.546162853cb3daffd64edd92014f274103f76360dfb39fc6e6ee399494da38fd.uk.png)](https://youtu.be/vieRiPRx-gI?si=cEZ8ApnT6Sus9rhn)

> _(Натисніть на зображення вище, щоб переглянути відео цього уроку)_

# Шаблон використання інструментів

Інструменти цікаві тим, що вони дозволяють AI-агентам мати ширший спектр можливостей. Замість того, щоб агент мав обмежений набір дій, які він може виконувати, додавання інструменту дозволяє агенту виконувати широкий спектр завдань. У цьому розділі ми розглянемо шаблон використання інструментів, який описує, як AI-агенти можуть використовувати конкретні інструменти для досягнення своїх цілей.

## Вступ

У цьому уроці ми прагнемо відповісти на такі запитання:

- Що таке шаблон використання інструментів?
- До яких випадків його можна застосувати?
- Які елементи/будівельні блоки потрібні для реалізації шаблону?
- Які особливі аспекти слід враховувати при використанні шаблону для створення надійних AI-агентів?

## Цілі навчання

Після завершення цього уроку ви зможете:

- Визначити шаблон використання інструментів та його призначення.
- Визначити випадки, де застосовний шаблон використання інструментів.
- Зрозуміти ключові елементи, необхідні для реалізації шаблону.
- Розпізнати аспекти, які забезпечують надійність AI-агентів при використанні цього шаблону.

## Що таке шаблон використання інструментів?

**Шаблон використання інструментів** зосереджується на наданні LLM можливості взаємодіяти із зовнішніми інструментами для досягнення конкретних цілей. Інструменти — це код, який може виконувати агент для здійснення дій. Інструмент може бути простою функцією, наприклад, калькулятором, або викликом API до стороннього сервісу, такого як пошук цін на акції чи прогноз погоди. У контексті AI-агентів інструменти розроблені для виконання агентами у відповідь на **виклики функцій, згенеровані моделлю**.

## До яких випадків його можна застосувати?

AI-агенти можуть використовувати інструменти для виконання складних завдань, отримання інформації або прийняття рішень. Шаблон використання інструментів часто застосовується в сценаріях, які потребують динамічної взаємодії із зовнішніми системами, такими як бази даних, веб-сервіси або інтерпретатори коду. Ця здатність корисна для багатьох випадків, зокрема:

- **Динамічне отримання інформації:** Агенти можуть запитувати зовнішні API або бази даних для отримання актуальних даних (наприклад, запит до бази SQLite для аналізу даних, отримання цін на акції або інформації про погоду).
- **Виконання та інтерпретація коду:** Агенти можуть виконувати код або скрипти для вирішення математичних задач, створення звітів або проведення симуляцій.
- **Автоматизація робочих процесів:** Автоматизація повторюваних або багатокрокових процесів шляхом інтеграції інструментів, таких як планувальники завдань, сервіси електронної пошти або конвеєри даних.
- **Підтримка клієнтів:** Агенти можуть взаємодіяти із CRM-системами, платформами для обробки запитів або базами знань для вирішення запитів користувачів.
- **Генерація та редагування контенту:** Агенти можуть використовувати інструменти, такі як перевірка граматики, підсумовування тексту або оцінка безпеки контенту для допомоги у створенні контенту.

## Які елементи/будівельні блоки потрібні для реалізації шаблону використання інструментів?

Ці будівельні блоки дозволяють AI-агенту виконувати широкий спектр завдань. Давайте розглянемо ключові елементи, необхідні для реалізації шаблону використання інструментів:

- **Схеми функцій/інструментів:** Детальні визначення доступних інструментів, включаючи назву функції, призначення, необхідні параметри та очікувані результати. Ці схеми дозволяють LLM зрозуміти, які інструменти доступні і як створювати коректні запити.

- **Логіка виконання функцій:** Визначає, як і коли інструменти викликаються на основі намірів користувача та контексту розмови. Це може включати модулі планування, механізми маршрутизації або умовні потоки, які динамічно визначають використання інструментів.

- **Система обробки повідомлень:** Компоненти, які керують потоком розмови між введенням користувача, відповідями LLM, викликами інструментів та їх результатами.

- **Фреймворк інтеграції інструментів:** Інфраструктура, яка з'єднує агента з різними інструментами, будь то прості функції або складні зовнішні сервіси.

- **Обробка помилок та перевірка:** Механізми для обробки збоїв у виконанні інструментів, перевірки параметрів та управління несподіваними відповідями.

- **Управління станом:** Відстежує контекст розмови, попередні взаємодії з інструментами та постійні дані для забезпечення узгодженості в багатокрокових взаємодіях.

Далі розглянемо виклики функцій/інструментів більш детально.

### Виклики функцій/інструментів

Виклик функцій — це основний спосіб, яким ми дозволяємо великим мовним моделям (LLM) взаємодіяти з інструментами. Ви часто побачите, що терміни "функція" і "інструмент" використовуються взаємозамінно, оскільки "функції" (блоки багаторазового коду) є "інструментами", які агенти використовують для виконання завдань. Щоб код функції був викликаний, LLM має порівняти запит користувача з описом функції. Для цього схема, що містить описи всіх доступних функцій, надсилається до LLM. Потім LLM вибирає найбільш відповідну функцію для завдання і повертає її назву та аргументи. Вибрана функція викликається, її відповідь повертається до LLM, який використовує інформацію для відповіді на запит користувача.

Для розробників, які хочуть реалізувати виклик функцій для агентів, вам знадобиться:

1. Модель LLM, яка підтримує виклик функцій
2. Схема, що містить описи функцій
3. Код для кожної описаної функції

Розглянемо приклад отримання поточного часу в місті:

1. **Ініціалізуйте LLM, яка підтримує виклик функцій:**

    Не всі моделі підтримують виклик функцій, тому важливо перевірити, чи підтримує це модель, яку ви використовуєте. <a href="https://learn.microsoft.com/azure/ai-services/openai/how-to/function-calling" target="_blank">Azure OpenAI</a> підтримує виклик функцій. Ми можемо почати з ініціалізації клієнта Azure OpenAI.

    ```python
    # Initialize the Azure OpenAI client
    client = AzureOpenAI(
        azure_endpoint = os.getenv("AZURE_OPENAI_ENDPOINT"), 
        api_key=os.getenv("AZURE_OPENAI_API_KEY"),  
        api_version="2024-05-01-preview"
    )
    ```

1. **Створіть схему функції:**

    Далі ми визначимо JSON-схему, яка містить назву функції, опис того, що вона робить, а також назви та описи параметрів функції. Потім ми передамо цю схему клієнту, створеному раніше, разом із запитом користувача знайти час у Сан-Франциско. Важливо зазначити, що повертається **виклик інструменту**, а не остаточна відповідь на запитання. Як згадувалося раніше, LLM повертає назву функції, яку вона вибрала для завдання, і аргументи, які будуть передані їй.

    ```python
    # Function description for the model to read
    tools = [
        {
            "type": "function",
            "function": {
                "name": "get_current_time",
                "description": "Get the current time in a given location",
                "parameters": {
                    "type": "object",
                    "properties": {
                        "location": {
                            "type": "string",
                            "description": "The city name, e.g. San Francisco",
                        },
                    },
                    "required": ["location"],
                },
            }
        }
    ]
    ```
   
    ```python
  
    # Initial user message
    messages = [{"role": "user", "content": "What's the current time in San Francisco"}] 
  
    # First API call: Ask the model to use the function
      response = client.chat.completions.create(
          model=deployment_name,
          messages=messages,
          tools=tools,
          tool_choice="auto",
      )
  
      # Process the model's response
      response_message = response.choices[0].message
      messages.append(response_message)
  
      print("Model's response:")  

      print(response_message)
  
    ```

    ```bash
    Model's response:
    ChatCompletionMessage(content=None, role='assistant', function_call=None, tool_calls=[ChatCompletionMessageToolCall(id='call_pOsKdUlqvdyttYB67MOj434b', function=Function(arguments='{"location":"San Francisco"}', name='get_current_time'), type='function')])
    ```
  
1. **Код функції, необхідний для виконання завдання:**

    Тепер, коли LLM вибрала, яку функцію потрібно виконати, необхідно реалізувати та виконати код, який виконує завдання. Ми можемо реалізувати код для отримання поточного часу на Python. Нам також потрібно написати код для вилучення назви та аргументів із response_message, щоб отримати остаточний результат.

    ```python
      def get_current_time(location):
        """Get the current time for a given location"""
        print(f"get_current_time called with location: {location}")  
        location_lower = location.lower()
        
        for key, timezone in TIMEZONE_DATA.items():
            if key in location_lower:
                print(f"Timezone found for {key}")  
                current_time = datetime.now(ZoneInfo(timezone)).strftime("%I:%M %p")
                return json.dumps({
                    "location": location,
                    "current_time": current_time
                })
      
        print(f"No timezone data found for {location_lower}")  
        return json.dumps({"location": location, "current_time": "unknown"})
    ```

     ```python
     # Handle function calls
      if response_message.tool_calls:
          for tool_call in response_message.tool_calls:
              if tool_call.function.name == "get_current_time":
     
                  function_args = json.loads(tool_call.function.arguments)
     
                  time_response = get_current_time(
                      location=function_args.get("location")
                  )
     
                  messages.append({
                      "tool_call_id": tool_call.id,
                      "role": "tool",
                      "name": "get_current_time",
                      "content": time_response,
                  })
      else:
          print("No tool calls were made by the model.")  
  
      # Second API call: Get the final response from the model
      final_response = client.chat.completions.create(
          model=deployment_name,
          messages=messages,
      )
  
      return final_response.choices[0].message.content
     ```

     ```bash
      get_current_time called with location: San Francisco
      Timezone found for san francisco
      The current time in San Francisco is 09:24 AM.
     ```

Виклик функцій є основою більшості, якщо не всіх, дизайнів використання інструментів агентами, однак його реалізація з нуля може бути складною. Як ми дізналися в [Уроці 2](../../../02-explore-agentic-frameworks), агентні фреймворки надають нам готові будівельні блоки для реалізації використання інструментів.

## Приклади використання інструментів із агентними фреймворками

Ось кілька прикладів того, як можна реалізувати шаблон використання інструментів за допомогою різних агентних фреймворків:

### Semantic Kernel

<a href="https://learn.microsoft.com/azure/ai-services/agents/overview" target="_blank">Semantic Kernel</a> — це відкритий AI-фреймворк для розробників .NET, Python і Java, які працюють із великими мовними моделями (LLM). Він спрощує процес використання виклику функцій, автоматично описуючи ваші функції та їх параметри моделі через процес, який називається <a href="https://learn.microsoft.com/semantic-kernel/concepts/ai-services/chat-completion/function-calling/?pivots=programming-language-python#1-serializing-the-functions" target="_blank">серіалізацією</a>. Він також керує зворотною комунікацією між моделлю та вашим кодом. Ще одна перевага використання агентного фреймворку, такого як Semantic Kernel, полягає в тому, що він дозволяє отримати доступ до готових інструментів, таких як <a href="https://github.com/microsoft/semantic-kernel/blob/main/python/samples/getting_started_with_agents/openai_assistant/step4_assistant_tool_file_search.py" target="_blank">Пошук файлів</a> і <a href="https://github.com/microsoft/semantic-kernel/blob/main/python/samples/getting_started_with_agents/openai_assistant/step3_assistant_tool_code_interpreter.py" target="_blank">Інтерпретатор коду</a>.

Наступна діаграма ілюструє процес виклику функцій із Semantic Kernel:

![виклик функцій](../../../translated_images/functioncalling-diagram.a84006fc287f60140cc0a484ff399acd25f69553ea05186981ac4d5155f9c2f6.uk.png)

У Semantic Kernel функції/інструменти називаються <a href="https://learn.microsoft.com/semantic-kernel/concepts/plugins/?pivots=programming-language-python" target="_blank">Плагінами</a>. Ми можемо перетворити функцію `get_current_time`, яку ми бачили раніше, на плагін, перетворивши її на клас із функцією всередині. Ми також можемо імпортувати декоратор `kernel_function`, який приймає опис функції. Коли ви створюєте ядро з GetCurrentTimePlugin, ядро автоматично серіалізує функцію та її параметри, створюючи схему для надсилання до LLM у процесі.

```python
from semantic_kernel.functions import kernel_function

class GetCurrentTimePlugin:
    async def __init__(self, location):
        self.location = location

    @kernel_function(
        description="Get the current time for a given location"
    )
    def get_current_time(location: str = ""):
        ...

```

```python 
from semantic_kernel import Kernel

# Create the kernel
kernel = Kernel()

# Create the plugin
get_current_time_plugin = GetCurrentTimePlugin(location)

# Add the plugin to the kernel
kernel.add_plugin(get_current_time_plugin)
```
  
### Azure AI Agent Service

<a href="https://learn.microsoft.com/azure/ai-services/agents/overview" target="_blank">Azure AI Agent Service</a> — це новий агентний фреймворк, розроблений для того, щоб допомогти розробникам безпечно створювати, розгортати та масштабувати якісних і розширюваних AI-агентів без необхідності керувати базовими обчислювальними та ресурсами зберігання. Він особливо корисний для корпоративних застосувань, оскільки є повністю керованим сервісом із корпоративним рівнем безпеки.

У порівнянні з розробкою безпосередньо через API LLM, Azure AI Agent Service надає деякі переваги, зокрема:

- Автоматичний виклик інструментів – немає необхідності аналізувати виклик інструменту, викликати інструмент і обробляти відповідь; усе це тепер виконується на сервері.
- Безпечно керовані дані – замість того, щоб керувати власним станом розмови, ви можете покладатися на потоки для зберігання всієї необхідної інформації.
- Готові інструменти – Інструменти, які можна використовувати для взаємодії з вашими джерелами даних, такі як Bing, Azure AI Search і Azure Functions.

Інструменти, доступні в Azure AI Agent Service, можна розділити на дві категорії:

1. Інструменти знань:
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/bing-grounding?tabs=python&pivots=overview" target="_blank">Пошук Bing</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/file-search?tabs=python&pivots=overview" target="_blank">Пошук файлів</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/azure-ai-search?tabs=azurecli%2Cpython&pivots=overview-azure-ai-search" target="_blank">Azure AI Search</a>

2. Інструменти дій:
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/function-calling?tabs=python&pivots=overview" target="_blank">Виклик функцій</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/code-interpreter?tabs=python&pivots=overview" target="_blank">Інтерпретатор коду</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/openapi-spec?tabs=python&pivots=overview" target="_blank">Інструменти, визначені OpenAI</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/azure-functions?pivots=overview" target="_blank">Azure Functions</a>

Сервіс агентів дозволяє використовувати ці інструменти разом як `toolset`. Він також використовує `threads`, які відстежують історію повідомлень із певної розмови.

Уявіть, що ви є торговим агентом у компанії Contoso. Ви хочете розробити розмовного агента, який може відповідати на запитання про ваші дані продажів.

Наступне зображення ілюструє, як можна використовувати Azure AI Agent Service для аналізу ваших даних продажів:

![Сервіс агентів у дії](../../../translated_images/agent-service-in-action.34fb465c9a84659edd3003f8cb62d6b366b310a09b37c44e32535021fbb5c93f.uk.jpg)

Щоб використовувати будь-який із цих інструментів із сервісом, ми можемо створити клієнта та визначити інструмент або набір інструментів. Для практичної реалізації ми можемо використовувати наступний код на Python. LLM зможе переглянути набір інструментів і вирішити, чи використовувати створену користувачем функцію `fetch_sales_data_using_sqlite_query`, чи попередньо створений Інтерпретатор коду залежно від запиту користувача.

```python 
import os
from azure.ai.projects import AIProjectClient
from azure.identity import DefaultAzureCredential
from fetch_sales_data_functions import fetch_sales_data_using_sqlite_query # fetch_sales_data_using_sqlite_query function which can be found in a fetch_sales_data_functions.py file.
from azure.ai.projects.models import ToolSet, FunctionTool, CodeInterpreterTool

project_client = AIProjectClient.from_connection_string(
    credential=DefaultAzureCredential(),
    conn_str=os.environ["PROJECT_CONNECTION_STRING"],
)

# Initialize function calling agent with the fetch_sales_data_using_sqlite_query function and adding it to the toolset
fetch_data_function = FunctionTool(fetch_sales_data_using_sqlite_query)
toolset = ToolSet()
toolset.add(fetch_data_function)

# Initialize Code Interpreter tool and adding it to the toolset. 
code_interpreter = code_interpreter = CodeInterpreterTool()
toolset = ToolSet()
toolset.add(code_interpreter)

agent = project_client.agents.create_agent(
    model="gpt-4o-mini", name="my-agent", instructions="You are helpful agent", 
    toolset=toolset
)
```

## Які особливі аспекти слід враховувати при використанні шаблону використання інструментів для створення надійних AI-агентів?

Поширене занепокоєння щодо SQL, динамічно створеного LLM, полягає в безпеці, зокрема ризику SQL-ін'єкцій або шкідливих дій, таких як видалення або зміна бази даних. Хоча ці занепокоєння є обґрунтованими, їх можна ефективно вирішити шляхом належного налаштування дозволів доступу до бази даних. Для більшості баз даних це передбачає налаштування бази даних як доступної лише для читання. Для таких сервісів баз даних, як PostgreSQL або Azure SQL, додатку слід призначити роль лише для читання (SELECT).

Запуск додатку в безпечному середовищі додатково підвищує захист. У корпоративних сценаріях дані зазвичай витягуються та трансформуються з операційних систем у
Приєднуйтесь до [Azure AI Foundry Discord](https://aka.ms/ai-agents/discord), щоб спілкуватися з іншими учасниками, відвідувати години консультацій та отримувати відповіді на ваші запитання щодо AI Agents.

## Додаткові ресурси

## Попередній урок

[Розуміння агентських шаблонів дизайну](../03-agentic-design-patterns/README.md)

## Наступний урок

[Агентський RAG](../05-agentic-rag/README.md)

---

**Відмова від відповідальності**:  
Цей документ було перекладено за допомогою сервісу автоматичного перекладу [Co-op Translator](https://github.com/Azure/co-op-translator). Хоча ми прагнемо до точності, будь ласка, майте на увазі, що автоматичні переклади можуть містити помилки або неточності. Оригінальний документ на його рідній мові слід вважати авторитетним джерелом. Для критично важливої інформації рекомендується професійний людський переклад. Ми не несемо відповідальності за будь-які непорозуміння або неправильні тлумачення, що виникають у результаті використання цього перекладу.