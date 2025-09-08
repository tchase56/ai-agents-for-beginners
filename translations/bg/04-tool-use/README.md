<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "4a5ccc4ad1dba85fbc2087cf3b986544",
  "translation_date": "2025-08-29T21:06:17+00:00",
  "source_file": "04-tool-use/README.md",
  "language_code": "bg"
}
-->
[![Как да проектираме добри AI агенти](../../../translated_images/lesson-4-thumbnail.546162853cb3daffd64edd92014f274103f76360dfb39fc6e6ee399494da38fd.bg.png)](https://youtu.be/vieRiPRx-gI?si=cEZ8ApnT6Sus9rhn)

> _(Кликнете върху изображението по-горе, за да гледате видеото към този урок)_

# Шаблон за проектиране на използване на инструменти

Инструментите са интересни, защото позволяват на AI агентите да имат по-широк набор от възможности. Вместо агентът да разполага с ограничен набор от действия, които може да изпълнява, добавянето на инструмент му позволява да извършва широк спектър от действия. В тази глава ще разгледаме шаблона за проектиране на използване на инструменти, който описва как AI агентите могат да използват специфични инструменти, за да постигнат целите си.

## Въведение

В този урок ще се опитаме да отговорим на следните въпроси:

- Какво представлява шаблонът за проектиране на използване на инструменти?
- За какви случаи на употреба може да се приложи?
- Какви са елементите/градивните блокове, необходими за прилагане на шаблона?
- Какви са специалните съображения при използването на шаблона за изграждане на надеждни AI агенти?

## Цели на обучението

След завършване на този урок ще можете:

- Да дефинирате шаблона за проектиране на използване на инструменти и неговата цел.
- Да идентифицирате случаи на употреба, при които шаблонът е приложим.
- Да разберете ключовите елементи, необходими за прилагане на шаблона.
- Да разпознавате съображенията за осигуряване на надеждност при AI агенти, използващи този шаблон.

## Какво представлява шаблонът за проектиране на използване на инструменти?

**Шаблонът за проектиране на използване на инструменти** се фокусира върху предоставянето на LLMs (Модели за големи езици) възможността да взаимодействат с външни инструменти за постигане на конкретни цели. Инструментите са код, който може да бъде изпълнен от агент за извършване на действия. Инструментът може да бъде проста функция, като калкулатор, или API повикване към услуга на трета страна, като проверка на цените на акции или прогноза за времето. В контекста на AI агентите инструментите са проектирани да бъдат изпълнявани от агенти в отговор на **генерирани от модела повиквания на функции**.

## За какви случаи на употреба може да се приложи?

AI агентите могат да използват инструменти за изпълнение на сложни задачи, извличане на информация или вземане на решения. Шаблонът за използване на инструменти често се използва в сценарии, изискващи динамично взаимодействие с външни системи, като бази данни, уеб услуги или интерпретатори на код. Тази способност е полезна за редица различни случаи на употреба, включително:

- **Динамично извличане на информация:** Агенти могат да правят заявки към външни API или бази данни за извличане на актуални данни (например, заявка към SQLite база данни за анализ на данни, извличане на цени на акции или информация за времето).
- **Изпълнение и интерпретация на код:** Агенти могат да изпълняват код или скриптове за решаване на математически задачи, генериране на отчети или извършване на симулации.
- **Автоматизация на работни процеси:** Автоматизиране на повтарящи се или многоетапни работни процеси чрез интегриране на инструменти като планировчици на задачи, имейл услуги или потоци от данни.
- **Поддръжка на клиенти:** Агенти могат да взаимодействат със CRM системи, платформи за билети или бази от знания за решаване на потребителски запитвания.
- **Генериране и редактиране на съдържание:** Агенти могат да използват инструменти като проверка на граматика, обобщаване на текст или оценка на безопасността на съдържанието за подпомагане на задачи, свързани със създаване на съдържание.

## Какви са елементите/градивните блокове, необходими за прилагане на шаблона за използване на инструменти?

Тези градивни блокове позволяват на AI агента да изпълнява широк спектър от задачи. Нека разгледаме ключовите елементи, необходими за прилагане на шаблона за използване на инструменти:

- **Схеми на функции/инструменти:** Подробни дефиниции на наличните инструменти, включително име на функцията, цел, изисквани параметри и очаквани изходи. Тези схеми позволяват на LLM да разбере какви инструменти са налични и как да създаде валидни заявки.
- **Логика за изпълнение на функции:** Определя как и кога инструментите се извикват въз основа на намерението на потребителя и контекста на разговора. Това може да включва модули за планиране, механизми за маршрутизиране или условни потоци, които динамично определят използването на инструменти.
- **Система за управление на съобщения:** Компоненти, които управляват потока на разговор между входовете на потребителя, отговорите на LLM, повикванията на инструменти и изходите на инструментите.
- **Рамка за интеграция на инструменти:** Инфраструктура, която свързва агента с различни инструменти, независимо дали са прости функции или сложни външни услуги.
- **Обработка на грешки и валидиране:** Механизми за справяне с неуспехи при изпълнение на инструменти, валидиране на параметри и управление на неочаквани отговори.
- **Управление на състоянието:** Проследява контекста на разговора, предишни взаимодействия с инструменти и постоянни данни, за да осигури последователност при многоходови взаимодействия.

След това ще разгледаме по-подробно извикването на функции/инструменти.

### Извикване на функции/инструменти

Извикването на функции е основният начин, по който позволяваме на LLMs да взаимодействат с инструменти. Често ще видите, че "функция" и "инструмент" се използват взаимозаменяемо, защото "функциите" (блокове от многократно използваем код) са "инструментите", които агентите използват за изпълнение на задачи. За да бъде извикан кодът на дадена функция, LLM трябва да сравни заявката на потребителя с описанието на функцията. За тази цел се изпраща схема, съдържаща описанията на всички налични функции, към LLM. След това LLM избира най-подходящата функция за задачата и връща нейното име и аргументи. Избраната функция се извиква, нейният отговор се изпраща обратно към LLM, който използва информацията, за да отговори на заявката на потребителя.

За да приложат извикване на функции за агенти, разработчиците ще се нуждаят от:

1. LLM модел, който поддържа извикване на функции
2. Схема, съдържаща описания на функциите
3. Кодът за всяка описана функция

Нека използваме примера с получаване на текущото време в даден град, за да илюстрираме:

1. **Инициализиране на LLM, който поддържа извикване на функции:**

    Не всички модели поддържат извикване на функции, затова е важно да проверите дали използваният от вас LLM го поддържа. <a href="https://learn.microsoft.com/azure/ai-services/openai/how-to/function-calling" target="_blank">Azure OpenAI</a> поддържа извикване на функции. Можем да започнем, като инициализираме клиента на Azure OpenAI.

    ```python
    # Initialize the Azure OpenAI client
    client = AzureOpenAI(
        azure_endpoint = os.getenv("AZURE_OPENAI_ENDPOINT"), 
        api_key=os.getenv("AZURE_OPENAI_API_KEY"),  
        api_version="2024-05-01-preview"
    )
    ```

1. **Създаване на схема на функция:**

    След това ще дефинираме JSON схема, която съдържа името на функцията, описание на това, което функцията прави, и имената и описанията на параметрите на функцията. Ще предадем тази схема на клиента, създаден по-рано, заедно със заявката на потребителя за намиране на времето в Сан Франциско. Важно е да се отбележи, че **извикване на инструмент** е това, което се връща, а **не** крайният отговор на въпроса. Както беше споменато по-рано, LLM връща името на функцията, която е избрал за задачата, и аргументите, които ще бъдат предадени на нея.

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
  
1. **Кодът на функцията, необходим за изпълнение на задачата:**

    След като LLM е избрал коя функция трябва да бъде изпълнена, кодът, който изпълнява задачата, трябва да бъде имплементиран и изпълнен. Можем да имплементираме кода за получаване на текущото време на Python. Също така ще трябва да напишем кода за извличане на името и аргументите от `response_message`, за да получим крайния резултат.

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

Извикването на функции е в основата на повечето, ако не и на всички дизайни за използване на инструменти от агенти, но имплементирането му от нулата понякога може да бъде предизвикателство. Както научихме в [Урок 2](../../../02-explore-agentic-frameworks), агентните рамки ни предоставят предварително изградени градивни блокове за имплементиране на използване на инструменти.

## Примери за използване на инструменти с агентни рамки

Ето някои примери за това как можете да имплементирате шаблона за използване на инструменти, използвайки различни агентни рамки:

### Semantic Kernel

<a href="https://learn.microsoft.com/azure/ai-services/agents/overview" target="_blank">Semantic Kernel</a> е отворена рамка за AI за разработчици на .NET, Python и Java, работещи с LLMs. Тя опростява процеса на използване на извикване на функции, като автоматично описва вашите функции и техните параметри на модела чрез процес, наречен <a href="https://learn.microsoft.com/semantic-kernel/concepts/ai-services/chat-completion/function-calling/?pivots=programming-language-python#1-serializing-the-functions" target="_blank">сериализация</a>. Тя също така управлява комуникацията между модела и вашия код. Друго предимство на използването на агентна рамка като Semantic Kernel е, че тя ви позволява да получите достъп до предварително изградени инструменти като <a href="https://github.com/microsoft/semantic-kernel/blob/main/python/samples/getting_started_with_agents/openai_assistant/step4_assistant_tool_file_search.py" target="_blank">Търсене на файлове</a> и <a href="https://github.com/microsoft/semantic-kernel/blob/main/python/samples/getting_started_with_agents/openai_assistant/step3_assistant_tool_code_interpreter.py" target="_blank">Интерпретатор на код</a>.

Следната диаграма илюстрира процеса на извикване на функции със Semantic Kernel:

![извикване на функции](../../../translated_images/functioncalling-diagram.a84006fc287f60140cc0a484ff399acd25f69553ea05186981ac4d5155f9c2f6.bg.png)

В Semantic Kernel функциите/инструментите се наричат <a href="https://learn.microsoft.com/semantic-kernel/concepts/plugins/?pivots=programming-language-python" target="_blank">плъгини</a>. Можем да преобразуваме функцията `get_current_time`, която видяхме по-рано, в плъгин, като я превърнем в клас с функцията в него. Можем също така да импортираме декоратора `kernel_function`, който приема описанието на функцията. Когато създадете ядро с плъгина GetCurrentTimePlugin, ядрото автоматично ще сериализира функцията и нейните параметри, създавайки схемата за изпращане към LLM в процеса.

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

<a href="https://learn.microsoft.com/azure/ai-services/agents/overview" target="_blank">Azure AI Agent Service</a> е по-нова агентна рамка, предназначена да даде възможност на разработчиците да изграждат, внедряват и мащабират висококачествени и разширяеми AI агенти, без да се налага да управляват основните изчислителни и съхранителни ресурси. Тя е особено полезна за корпоративни приложения, тъй като е напълно управлявана услуга с корпоративна степен на сигурност.

В сравнение с разработването директно с LLM API, Azure AI Agent Service предоставя някои предимства, включително:

- Автоматично извикване на инструменти – няма нужда да анализирате извикване на инструмент, да извиквате инструмента и да обработвате отговора; всичко това вече се извършва на сървърната страна.
- Сигурно управлявани данни – вместо да управлявате собственото си състояние на разговор, можете да разчитате на нишки за съхранение на цялата необходима информация.
- Готови за използване инструменти – Инструменти, които можете да използвате за взаимодействие с вашите източници на данни, като Bing, Azure AI Search и Azure Functions.

Инструментите, налични в Azure AI Agent Service, могат да бъдат разделени на две категории:

1. Инструменти за знания:
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/bing-grounding?tabs=python&pivots=overview" target="_blank">Основа с Bing Search</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/file-search?tabs=python&pivots=overview" target="_blank">Търсене на файлове</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/azure-ai-search?tabs=azurecli%2Cpython&pivots=overview-azure-ai-search" target="_blank">Azure AI Search</a>

2. Инструменти за действия:
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/function-calling?tabs=python&pivots=overview" target="_blank">Извикване на функции</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/code-interpreter?tabs=python&pivots=overview" target="_blank">Интерпретатор на код</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/openapi-spec?tabs=python&pivots=overview" target="_blank">Инструменти, дефинирани от OpenAI</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/azure-functions?pivots=overview" target="_blank">Azure Functions</a>

Agent Service ни позволява да използваме тези инструменти заедно като `toolset`. Тя също така използва `threads`, които проследяват историята на съобщенията от конкретен разговор.

Представете си, че сте търговски агент в компания, наречена Contoso. Искате да разработите разговорен агент, който може да отговаря на въпроси относно вашите търговски данни.

Следното изображение илюстрира как можете да използвате Azure AI Agent Service за анализ на вашите търговски данни:

![Agentic Service в действие](../../../translated_images/agent-service-in-action.34fb465c9a84659edd3003f8cb62d6b366b310a09b37c44e32535021fbb5c93f.bg.jpg)

За да използвате някой от тези инструменти със услугата, можем да създадем клиент и да дефинираме инструмент или набор от инструменти. За да го имплементираме практически, можем да използваме следния Python код. LLM ще може да разгледа набора от инструменти и да реши дали да използва създадената от потребителя функция `fetch_sales_data_using_sqlite_query` или предварително изградения интерпретатор на код в зависимост от заявката на потребителя.

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

## Какви са специалните съображения при използването на шаблона за проектиране на използване на инструменти за изграждане на надеждни AI агенти?

Често срещано притеснение при SQL, генери
Присъединете се към [Azure AI Foundry Discord](https://aka.ms/ai-agents/discord), за да се срещнете с други обучаващи се, да присъствате на консултации и да получите отговори на вашите въпроси относно AI агенти.

## Допълнителни ресурси

## Предишен урок

[Разбиране на агентни дизайнерски модели](../03-agentic-design-patterns/README.md)

## Следващ урок

[Агентен RAG](../05-agentic-rag/README.md)

---

**Отказ от отговорност**:  
Този документ е преведен с помощта на AI услуга за превод [Co-op Translator](https://github.com/Azure/co-op-translator). Въпреки че се стремим към точност, моля, имайте предвид, че автоматизираните преводи може да съдържат грешки или неточности. Оригиналният документ на неговия роден език трябва да се счита за авторитетен източник. За критична информация се препоръчва професионален човешки превод. Ние не носим отговорност за каквито и да е недоразумения или погрешни интерпретации, произтичащи от използването на този превод.