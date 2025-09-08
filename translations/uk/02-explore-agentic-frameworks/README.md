<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-29T23:46:00+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "uk"
}
-->
[![Дослідження фреймворків AI агентів](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.uk.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(Натисніть на зображення вище, щоб переглянути відео цього уроку)_

# Дослідження фреймворків AI агентів

Фреймворки AI агентів — це програмні платформи, створені для спрощення розробки, розгортання та управління AI агентами. Вони надають розробникам готові компоненти, абстракції та інструменти, які полегшують створення складних AI систем.

Ці фреймворки допомагають розробникам зосередитися на унікальних аспектах їхніх застосунків, пропонуючи стандартизовані підходи до вирішення загальних викликів у розробці AI агентів. Вони підвищують масштабованість, доступність та ефективність у створенні AI систем.

## Вступ

Цей урок охоплює:

- Що таке фреймворки AI агентів і що вони дозволяють розробникам досягти?
- Як команди можуть використовувати їх для швидкого прототипування, ітерації та покращення можливостей своїх агентів?
- У чому різниця між фреймворками та інструментами, створеними Microsoft, OpenAI та іншими?
- Чи можу я інтегрувати свої існуючі інструменти Azure екосистеми безпосередньо, чи потрібні окремі рішення?
- Що таке Azure AI Agents Service і як це може допомогти мені?

## Цілі навчання

Цілі цього уроку допоможуть вам зрозуміти:

- Роль фреймворків AI агентів у розробці AI.
- Як використовувати фреймворки AI агентів для створення інтелектуальних агентів.
- Основні можливості, які забезпечують фреймворки AI агентів.
- Відмінності між AutoGen, Semantic Kernel та Azure AI Agent Service.

## Що таке фреймворки AI агентів і що вони дозволяють розробникам робити?

Традиційні AI фреймворки можуть допомогти інтегрувати AI у ваші застосунки та покращити їх у таких аспектах:

- **Персоналізація**: AI може аналізувати поведінку користувачів і їхні вподобання, щоб надавати персоналізовані рекомендації, контент і досвід.
  Приклад: Стрімінгові сервіси, такі як Netflix, використовують AI для пропонування фільмів і шоу на основі історії переглядів, підвищуючи залученість і задоволення користувачів.
- **Автоматизація та ефективність**: AI може автоматизувати повторювані завдання, оптимізувати робочі процеси та підвищувати операційну ефективність.
  Приклад: Додатки для обслуговування клієнтів використовують AI-чатботів для обробки поширених запитів, скорочуючи час відповіді та звільняючи людських агентів для вирішення складніших питань.
- **Покращений користувацький досвід**: AI може покращити загальний досвід користувачів, надаючи інтелектуальні функції, такі як розпізнавання голосу, обробка природної мови та передбачуваний текст.
  Приклад: Віртуальні асистенти, такі як Siri та Google Assistant, використовують AI для розуміння та реагування на голосові команди, полегшуючи взаємодію користувачів із пристроями.

### Це звучить чудово, але чому нам потрібен фреймворк AI агентів?

Фреймворки AI агентів представляють щось більше, ніж просто AI фреймворки. Вони створені для розробки інтелектуальних агентів, які можуть взаємодіяти з користувачами, іншими агентами та середовищем для досягнення конкретних цілей. Ці агенти можуть демонструвати автономну поведінку, приймати рішення та адаптуватися до змінних умов. Ось деякі ключові можливості, які забезпечують фреймворки AI агентів:

- **Співпраця та координація агентів**: Дозволяють створювати кілька AI агентів, які можуть працювати разом, спілкуватися та координувати свої дії для вирішення складних завдань.
- **Автоматизація та управління завданнями**: Забезпечують механізми для автоматизації багатокрокових робочих процесів, делегування завдань і динамічного управління завданнями серед агентів.
- **Контекстуальне розуміння та адаптація**: Оснащують агентів здатністю розуміти контекст, адаптуватися до змін у середовищі та приймати рішення на основі інформації в реальному часі.

Отже, підсумовуючи, агенти дозволяють робити більше, піднімати автоматизацію на новий рівень, створювати більш інтелектуальні системи, які можуть адаптуватися та навчатися від свого середовища.

## Як швидко прототипувати, ітерувати та покращувати можливості агентів?

Це швидко змінюваний ландшафт, але є деякі речі, які є спільними для більшості фреймворків AI агентів і які можуть допомогти вам швидко прототипувати та ітерувати, а саме модульні компоненти, інструменти для співпраці та навчання в реальному часі. Давайте розглянемо ці аспекти:

- **Використовуйте модульні компоненти**: SDK AI пропонують готові компоненти, такі як AI і Memory конектори, виклик функцій за допомогою природної мови або плагінів коду, шаблони підказок тощо.
- **Використовуйте інструменти для співпраці**: Проектуйте агентів із конкретними ролями та завданнями, що дозволяє тестувати та вдосконалювати робочі процеси співпраці.
- **Навчайтеся в реальному часі**: Реалізуйте зворотні зв’язки, де агенти навчаються на взаємодіях і динамічно коригують свою поведінку.

### Використовуйте модульні компоненти

SDK, такі як Microsoft Semantic Kernel і LangChain, пропонують готові компоненти, такі як AI конектори, шаблони підказок і управління пам’яттю.

**Як команди можуть це використовувати**: Команди можуть швидко зібрати ці компоненти, щоб створити функціональний прототип без необхідності починати з нуля, що дозволяє швидко експериментувати та ітерувати.

**Як це працює на практиці**: Ви можете використовувати готовий парсер для вилучення інформації з введення користувача, модуль пам’яті для зберігання та отримання даних і генератор підказок для взаємодії з користувачами, не створюючи ці компоненти з нуля.

**Приклад коду**. Давайте розглянемо приклади використання готового AI конектора з Semantic Kernel Python і .Net, який використовує автоматичний виклик функцій для відповіді моделі на введення користувача:

``` python
# Semantic Kernel Python Example

import asyncio
from typing import Annotated

from semantic_kernel.connectors.ai import FunctionChoiceBehavior
from semantic_kernel.connectors.ai.open_ai import AzureChatCompletion, AzureChatPromptExecutionSettings
from semantic_kernel.contents import ChatHistory
from semantic_kernel.functions import kernel_function
from semantic_kernel.kernel import Kernel

# Define a ChatHistory object to hold the conversation's context
chat_history = ChatHistory()
chat_history.add_user_message("I'd like to go to New York on January 1, 2025")


# Define a sample plugin that contains the function to book travel
class BookTravelPlugin:
    """A Sample Book Travel Plugin"""

    @kernel_function(name="book_flight", description="Book travel given location and date")
    async def book_flight(
        self, date: Annotated[str, "The date of travel"], location: Annotated[str, "The location to travel to"]
    ) -> str:
        return f"Travel was booked to {location} on {date}"

# Create the Kernel
kernel = Kernel()

# Add the sample plugin to the Kernel object
kernel.add_plugin(BookTravelPlugin(), plugin_name="book_travel")

# Define the Azure OpenAI AI Connector
chat_service = AzureChatCompletion(
    deployment_name="YOUR_DEPLOYMENT_NAME", 
    api_key="YOUR_API_KEY", 
    endpoint="https://<your-resource>.azure.openai.com/",
)

# Define the request settings to configure the model with auto-function calling
request_settings = AzureChatPromptExecutionSettings(function_choice_behavior=FunctionChoiceBehavior.Auto())


async def main():
    # Make the request to the model for the given chat history and request settings
    # The Kernel contains the sample that the model will request to invoke
    response = await chat_service.get_chat_message_content(
        chat_history=chat_history, settings=request_settings, kernel=kernel
    )
    assert response is not None

    """
    Note: In the auto function calling process, the model determines it can invoke the 
    `BookTravelPlugin` using the `book_flight` function, supplying the necessary arguments. 
    
    For example:

    "tool_calls": [
        {
            "id": "call_abc123",
            "type": "function",
            "function": {
                "name": "BookTravelPlugin-book_flight",
                "arguments": "{'location': 'New York', 'date': '2025-01-01'}"
            }
        }
    ]

    Since the location and date arguments are required (as defined by the kernel function), if the 
    model lacks either, it will prompt the user to provide them. For instance:

    User: Book me a flight to New York.
    Model: Sure, I'd love to help you book a flight. Could you please specify the date?
    User: I want to travel on January 1, 2025.
    Model: Your flight to New York on January 1, 2025, has been successfully booked. Safe travels!
    """

    print(f"`{response}`")
    # Example AI Model Response: `Your flight to New York on January 1, 2025, has been successfully booked. Safe travels! ✈️🗽`

    # Add the model's response to our chat history context
    chat_history.add_assistant_message(response.content)


if __name__ == "__main__":
    asyncio.run(main())
```
```csharp
// Semantic Kernel C# example

using Microsoft.SemanticKernel;
using Microsoft.SemanticKernel.ChatCompletion;
using System.ComponentModel;
using Microsoft.SemanticKernel.Connectors.AzureOpenAI;

ChatHistory chatHistory = [];
chatHistory.AddUserMessage("I'd like to go to New York on January 1, 2025");

var kernelBuilder = Kernel.CreateBuilder();
kernelBuilder.AddAzureOpenAIChatCompletion(
    deploymentName: "NAME_OF_YOUR_DEPLOYMENT",
    apiKey: "YOUR_API_KEY",
    endpoint: "YOUR_AZURE_ENDPOINT"
);
kernelBuilder.Plugins.AddFromType<BookTravelPlugin>("BookTravel"); 
var kernel = kernelBuilder.Build();

var settings = new AzureOpenAIPromptExecutionSettings()
{
    FunctionChoiceBehavior = FunctionChoiceBehavior.Auto()
};

var chatCompletion = kernel.GetRequiredService<IChatCompletionService>();

var response = await chatCompletion.GetChatMessageContentAsync(chatHistory, settings, kernel);

/*
Behind the scenes, the model recognizes the tool to call, what arguments it already has (location) and (date)
{

"tool_calls": [
    {
        "id": "call_abc123",
        "type": "function",
        "function": {
            "name": "BookTravelPlugin-book_flight",
            "arguments": "{'location': 'New York', 'date': '2025-01-01'}"
        }
    }
]
*/

Console.WriteLine(response.Content);
chatHistory.AddMessage(response!.Role, response!.Content!);

// Example AI Model Response: Your flight to New York on January 1, 2025, has been successfully booked. Safe travels! ✈️🗽

// Define a plugin that contains the function to book travel
public class BookTravelPlugin
{
    [KernelFunction("book_flight")]
    [Description("Book travel given location and date")]
    public async Task<string> BookFlight(DateTime date, string location)
    {
        return await Task.FromResult( $"Travel was booked to {location} on {date}");
    }
}
```

З цього прикладу видно, як можна використовувати готовий парсер для вилучення ключової інформації з введення користувача, наприклад, місця відправлення, призначення та дати запиту на бронювання рейсу. Цей модульний підхід дозволяє зосередитися на високорівневій логіці.

### Використовуйте інструменти для співпраці

Фреймворки, такі як CrewAI, Microsoft AutoGen і Semantic Kernel, сприяють створенню кількох агентів, які можуть працювати разом.

**Як команди можуть це використовувати**: Команди можуть проектувати агентів із конкретними ролями та завданнями, що дозволяє тестувати та вдосконалювати робочі процеси співпраці та підвищувати загальну ефективність системи.

**Як це працює на практиці**: Ви можете створити команду агентів, де кожен агент має спеціалізовану функцію, наприклад, отримання даних, аналіз або прийняття рішень. Ці агенти можуть спілкуватися та обмінюватися інформацією для досягнення спільної мети, наприклад, відповіді на запит користувача або виконання завдання.

**Приклад коду (AutoGen)**:

```python
# creating agents, then create a round robin schedule where they can work together, in this case in order

# Data Retrieval Agent
# Data Analysis Agent
# Decision Making Agent

agent_retrieve = AssistantAgent(
    name="dataretrieval",
    model_client=model_client,
    tools=[retrieve_tool],
    system_message="Use tools to solve tasks."
)

agent_analyze = AssistantAgent(
    name="dataanalysis",
    model_client=model_client,
    tools=[analyze_tool],
    system_message="Use tools to solve tasks."
)

# conversation ends when user says "APPROVE"
termination = TextMentionTermination("APPROVE")

user_proxy = UserProxyAgent("user_proxy", input_func=input)

team = RoundRobinGroupChat([agent_retrieve, agent_analyze, user_proxy], termination_condition=termination)

stream = team.run_stream(task="Analyze data", max_turns=10)
# Use asyncio.run(...) when running in a script.
await Console(stream)
```

У попередньому коді показано, як можна створити завдання, яке передбачає співпрацю кількох агентів для аналізу даних. Кожен агент виконує певну функцію, а завдання виконується шляхом координації агентів для досягнення бажаного результату. Створюючи спеціалізованих агентів із конкретними ролями, ви можете підвищити ефективність і продуктивність завдань.

### Навчайтеся в реальному часі

Розширені фреймворки забезпечують можливості для розуміння контексту в реальному часі та адаптації.

**Як команди можуть це використовувати**: Команди можуть реалізувати зворотні зв’язки, де агенти навчаються на взаємодіях і динамічно коригують свою поведінку, що призводить до постійного вдосконалення та розширення можливостей.

**Як це працює на практиці**: Агенти можуть аналізувати відгуки користувачів, дані середовища та результати завдань, щоб оновлювати свою базу знань, коригувати алгоритми прийняття рішень і покращувати продуктивність з часом. Цей ітеративний процес навчання дозволяє агентам адаптуватися до змінних умов і вподобань користувачів, підвищуючи загальну ефективність системи.

## У чому різниця між фреймворками AutoGen, Semantic Kernel і Azure AI Agent Service?

Існує багато способів порівняти ці фреймворки, але давайте розглянемо деякі ключові відмінності з точки зору їхнього дизайну, можливостей і цільових сценаріїв використання:

## AutoGen

AutoGen — це фреймворк з відкритим кодом, розроблений AI Frontiers Lab Microsoft Research. Він зосереджений на подієво-орієнтованих, розподілених *агентних* застосунках, що дозволяють використовувати кілька LLMs і SLMs, інструменти та розширені шаблони дизайну мультиагентних систем.

AutoGen побудований навколо основної концепції агентів, які є автономними сутностями, здатними сприймати своє середовище, приймати рішення та виконувати дії для досягнення конкретних цілей. Агенти спілкуються через асинхронні повідомлення, що дозволяє їм працювати незалежно та паралельно, підвищуючи масштабованість і чутливість системи.

Згідно з Wikipedia, актор — це _основний будівельний блок паралельних обчислень. У відповідь на отримане повідомлення актор може: приймати локальні рішення, створювати більше акторів, надсилати більше повідомлень і визначати, як реагувати на наступне отримане повідомлення_.

**Сценарії використання**: Автоматизація генерації коду, завдання аналізу даних і створення користувацьких агентів для функцій планування та дослідження.

Ось деякі важливі основні концепції AutoGen:

- **Агенти**. Агент — це програмна сутність, яка:
  - **Спілкується через повідомлення**, які можуть бути синхронними або асинхронними.
  - **Підтримує власний стан**, який може змінюватися вхідними повідомленнями.
  - **Виконує дії** у відповідь на отримані повідомлення або зміни у своєму стані. Ці дії можуть змінювати стан агента та створювати зовнішні ефекти, такі як оновлення журналів повідомлень, надсилання нових повідомлень, виконання коду або виклики API.

  Ось короткий приклад коду, у якому ви створюєте власного агента з можливостями чату:

    ```python
    from autogen_agentchat.agents import AssistantAgent
    from autogen_agentchat.messages import TextMessage
    from autogen_ext.models.openai import OpenAIChatCompletionClient


    class MyAssistant(RoutedAgent):
        def __init__(self, name: str) -> None:
            super().__init__(name)
            model_client = OpenAIChatCompletionClient(model="gpt-4o")
            self._delegate = AssistantAgent(name, model_client=model_client)
    
        @message_handler
        async def handle_my_message_type(self, message: MyMessageType, ctx: MessageContext) -> None:
            print(f"{self.id.type} received message: {message.content}")
            response = await self._delegate.on_messages(
                [TextMessage(content=message.content, source="user")], ctx.cancellation_token
            )
            print(f"{self.id.type} responded: {response.chat_message.content}")
    ```
    
    У попередньому коді створено `MyAssistant`, який успадковується від `RoutedAgent`. Він має обробник повідомлень, який друкує вміст повідомлення, а потім надсилає відповідь за допомогою делегата `AssistantAgent`. Особливо зверніть увагу, як ми призначаємо `self._delegate` екземпляр `AssistantAgent`, який є готовим агентом, здатним обробляти завершення чату.

    Давайте повідомимо AutoGen про цей тип агента та запустимо програму:

    ```python
    
    # main.py
    runtime = SingleThreadedAgentRuntime()
    await MyAgent.register(runtime, "my_agent", lambda: MyAgent())

    runtime.start()  # Start processing messages in the background.
    await runtime.send_message(MyMessageType("Hello, World!"), AgentId("my_agent", "default"))
    ```

    У попередньому коді агенти реєструються в середовищі виконання, а потім агенту надсилається повідомлення, що призводить до наступного результату:

    ```text
    # Output from the console:
    my_agent received message: Hello, World!
    my_assistant received message: Hello, World!
    my_assistant responded: Hello! How can I assist you today?
    ```

- **Мультиагенти**. AutoGen підтримує створення кількох агентів, які можуть працювати разом для досягнення складних завдань. Агенти можуть спілкуватися, обмінюватися інформацією та координувати свої дії для більш ефективного вирішення проблем. Щоб створити мультиагентну систему, ви можете визначити різні типи агентів із спеціалізованими функціями та ролями, такими як отримання даних, аналіз, прийняття рішень і взаємодія з користувачем. Давайте подивимося, як виглядає таке створення:

    ```python
    editor_description = "Editor for planning and reviewing the content."

    # Example of declaring an Agent
    editor_agent_type = await EditorAgent.register(
    runtime,
    editor_topic_type,  # Using topic type as the agent type.
    lambda: EditorAgent(
        description=editor_description,
        group_chat_topic_type=group_chat_topic_type,
        model_client=OpenAIChatCompletionClient(
            model="gpt-4o-2024-08-06",
            # api_key="YOUR_API_KEY",
        ),
        ),
    )

    # remaining declarations shortened for brevity

    # Group chat
    group_chat_manager_type = await GroupChatManager.register(
    runtime,
    "group_chat_manager",
    lambda: GroupChatManager(
        participant_topic_types=[writer_topic_type, illustrator_topic_type, editor_topic_type, user_topic_type],
        model_client=OpenAIChatCompletionClient(
            model="gpt-4o-2024-08-06",
            # api_key="YOUR_API_KEY",
        ),
        participant_descriptions=[
            writer_description, 
            illustrator_description, 
            editor_description, 
            user_description
        ],
        ),
    )
    ```

    У попередньому коді ми маємо `GroupChatManager`, який зареєстрований у середовищі виконання. Цей менеджер відповідає за координацію взаємодій між різними типами агентів, такими як письменники, ілюстратори, редактори та користувачі.

- **Середовище виконання агентів**. Фреймворк надає середовище виконання, яке забезпечує зв’язок між агентами, керує їхніми ідентифікаторами та життєвими циклами, а також забезпечує дотримання меж безпеки та конфіденційності. Це означає, що ви можете запускати своїх агентів у безпечному та контрольованому середовищі, забезпечуючи їхню безпечну та ефективну взаємодію. Існує два середовища виконання, які заслуговують на увагу:
  - **Автономне середовище виконання**. Це хороший вибір для однопроцесних застосунків, де всі агенти реалізовані однією мовою програмування та працюють у тому самому процесі. Ось ілюстрація того, як це працює:

    Стек застосунків

    *агенти спілкуються через повідомлення через середовище виконання, яке керує життєвим циклом агентів*

  - **Розподілене середовище виконання агентів**, підходить для багатопроцесних застосунків, де агенти можуть бути реалізовані різними мовами програмування та працювати на різних машинах. Ось ілюстрація того, як це працює:

## Semantic Kernel + Agent Framework

Semantic Kernel — це SDK для оркестрації AI, готовий до використання в корпоративному середовищі. Він складається з AI і Memory конекторів, а також фреймворку агентів.

Спочатку розглянемо деякі основні компоненти:

- **AI конектори**: Це інтерфейс із зовнішніми AI сервісами та джерелами даних для використання як у Python, так і в C#.

  ```python
  # Semantic Kernel Python
  from semantic_kernel.connectors.ai.open_ai import AzureChatCompletion
  from semantic_kernel.kernel import Kernel

  kernel = Kernel()
  kernel.add_service(
    AzureChatCompletion(
        deployment_name="your-deployment-name",
        api_key="your-api-key",
        endpoint="your-endpoint",
    )
  )
  ```  

    ```csharp
    // Semantic Kernel C#
    using Microsoft.SemanticKernel;

    // Create kernel
    var builder = Kernel.CreateBuilder();
    
    // Add a chat completion service:
    builder.Services.AddAzureOpenAIChatCompletion(
        "your-resource-name",
        "your-endpoint",
        "your-resource-key",
        "deployment-model");
    var kernel = builder.Build();
    ```

    Ось простий приклад того, як можна створити ядро та додати сервіс завершення чату. Semantic Kernel створює з’єднання із зовнішнім AI сервісом, у цьому випадку Azure OpenAI Chat Completion.

- **Плагіни**: Вони інкапсулюють функції, які може використовувати застосунок. Є як готові плагіни, так і ті, які ви можете створити самостійно. Суміжною концепцією є "функції підказок". Замість надання природних мовних підказок для виклику функцій, ви транслюєте певні функції до моделі. На основі поточного контексту чату модель може вибрати виклик однієї з цих функцій для виконання запиту чи запитання. Ось приклад:

  ```python
  from semantic_kernel.connectors.ai.open_ai.services.azure_chat_completion import AzureChatCompletion


  async def main():
      from semantic_kernel.functions import KernelFunctionFromPrompt
      from semantic_kernel.kernel import Kernel

      kernel = Kernel()
      kernel.add_service(AzureChatCompletion())

      user_input = input("User Input:> ")

      kernel_function = KernelFunctionFromPrompt(
          function_name="SummarizeText",
          prompt="""
          Summarize the provided unstructured text in a sentence that is easy to understand.
          Text to summarize: {{$user_input}}
          """,
      )

      response = await kernel_function.invoke(kernel=kernel, user_input=user_input)
      print(f"Model Response: {response}")

      """
      Sample Console Output:

      User Input:> I like dogs
      Model Response: The text expresses a preference for dogs.
      """


  if __name__ == "__main__":
    import asyncio
    asyncio.run(main())
  ```

    ```csharp
    var userInput = Console.ReadLine();

    // Define semantic function inline.
    string skPrompt = @"Summarize the provided unstructured text in a sentence that is easy to understand.
                        Text to summarize: {{$userInput}}";
    
    // create the function from the prompt
    KernelFunction summarizeFunc = kernel.CreateFunctionFromPrompt(
        promptTemplate: skPrompt,
        functionName: "SummarizeText"
    );

    //then import into the current kernel
    kernel.ImportPluginFromFunctions("SemanticFunctions", [summarizeFunc]);

    ```

    Тут спочатку є
Отже, це основи фреймворку Semantic Kernel, а як щодо Agent Framework?

## Azure AI Agent Service

Azure AI Agent Service — це нове доповнення, представлене на Microsoft Ignite 2024. Воно дозволяє розробляти та розгортати AI-агентів із більш гнучкими моделями, такими як прямий виклик відкритих LLM, наприклад, Llama 3, Mistral і Cohere.

Azure AI Agent Service забезпечує потужніші механізми безпеки для підприємств і методи зберігання даних, що робить його придатним для корпоративних застосувань.

Він працює "з коробки" з фреймворками оркестрації мультиагентів, такими як AutoGen і Semantic Kernel.

Ця служба наразі перебуває у стадії Public Preview і підтримує Python та C# для створення агентів.

Використовуючи Semantic Kernel Python, ми можемо створити Azure AI Agent із плагіном, визначеним користувачем:

```python
import asyncio
from typing import Annotated

from azure.identity.aio import DefaultAzureCredential

from semantic_kernel.agents import AzureAIAgent, AzureAIAgentSettings, AzureAIAgentThread
from semantic_kernel.contents import ChatMessageContent
from semantic_kernel.contents import AuthorRole
from semantic_kernel.functions import kernel_function


# Define a sample plugin for the sample
class MenuPlugin:
    """A sample Menu Plugin used for the concept sample."""

    @kernel_function(description="Provides a list of specials from the menu.")
    def get_specials(self) -> Annotated[str, "Returns the specials from the menu."]:
        return """
        Special Soup: Clam Chowder
        Special Salad: Cobb Salad
        Special Drink: Chai Tea
        """

    @kernel_function(description="Provides the price of the requested menu item.")
    def get_item_price(
        self, menu_item: Annotated[str, "The name of the menu item."]
    ) -> Annotated[str, "Returns the price of the menu item."]:
        return "$9.99"


async def main() -> None:
    ai_agent_settings = AzureAIAgentSettings.create()

    async with (
        DefaultAzureCredential() as creds,
        AzureAIAgent.create_client(
            credential=creds,
            conn_str=ai_agent_settings.project_connection_string.get_secret_value(),
        ) as client,
    ):
        # Create agent definition
        agent_definition = await client.agents.create_agent(
            model=ai_agent_settings.model_deployment_name,
            name="Host",
            instructions="Answer questions about the menu.",
        )

        # Create the AzureAI Agent using the defined client and agent definition
        agent = AzureAIAgent(
            client=client,
            definition=agent_definition,
            plugins=[MenuPlugin()],
        )

        # Create a thread to hold the conversation
        # If no thread is provided, a new thread will be
        # created and returned with the initial response
        thread: AzureAIAgentThread | None = None

        user_inputs = [
            "Hello",
            "What is the special soup?",
            "How much does that cost?",
            "Thank you",
        ]

        try:
            for user_input in user_inputs:
                print(f"# User: '{user_input}'")
                # Invoke the agent for the specified thread
                response = await agent.get_response(
                    messages=user_input,
                    thread_id=thread,
                )
                print(f"# {response.name}: {response.content}")
                thread = response.thread
        finally:
            await thread.delete() if thread else None
            await client.agents.delete_agent(agent.id)


if __name__ == "__main__":
    asyncio.run(main())
```

### Основні концепції

Azure AI Agent Service має такі основні концепції:

- **Агент**. Azure AI Agent Service інтегрується з Azure AI Foundry. У межах AI Foundry AI-агент діє як "розумний" мікросервіс, який можна використовувати для відповідей на запитання (RAG), виконання дій або повної автоматизації робочих процесів. Це досягається шляхом поєднання потужності генеративних AI-моделей з інструментами, які дозволяють отримувати доступ до реальних джерел даних і взаємодіяти з ними. Ось приклад агента:

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    У цьому прикладі створюється агент із моделлю `gpt-4o-mini`, ім'ям `my-agent` та інструкціями `You are helpful agent`. Агент оснащений інструментами та ресурсами для виконання завдань інтерпретації коду.

- **Тред і повідомлення**. Тред — це ще одна важлива концепція. Він представляє розмову або взаємодію між агентом і користувачем. Треди можна використовувати для відстеження прогресу розмови, зберігання контекстної інформації та управління станом взаємодії. Ось приклад треду:

    ```python
    thread = project_client.agents.create_thread()
    message = project_client.agents.create_message(
        thread_id=thread.id,
        role="user",
        content="Could you please create a bar chart for the operating profit using the following data and provide the file to me? Company A: $1.2 million, Company B: $2.5 million, Company C: $3.0 million, Company D: $1.8 million",
    )
    
    # Ask the agent to perform work on the thread
    run = project_client.agents.create_and_process_run(thread_id=thread.id, agent_id=agent.id)
    
    # Fetch and log all messages to see the agent's response
    messages = project_client.agents.list_messages(thread_id=thread.id)
    print(f"Messages: {messages}")
    ```

    У попередньому коді створюється тред. Потім до треду надсилається повідомлення. Викликом `create_and_process_run` агенту доручається виконати роботу над тредом. Нарешті, повідомлення отримуються та записуються в лог, щоб побачити відповідь агента. Повідомлення вказують на прогрес розмови між користувачем і агентом. Також важливо розуміти, що повідомлення можуть бути різних типів, таких як текст, зображення або файл, тобто робота агента може призвести, наприклад, до створення зображення або текстової відповіді. Як розробник, ви можете використовувати цю інформацію для подальшої обробки відповіді або її представлення користувачеві.

- **Інтеграція з іншими AI-фреймворками**. Azure AI Agent Service може взаємодіяти з іншими фреймворками, такими як AutoGen і Semantic Kernel, що означає, що ви можете створити частину свого застосунку в одному з цих фреймворків, використовуючи Agent Service як оркестратор, або створити все в Agent Service.

**Випадки використання**: Azure AI Agent Service розроблений для корпоративних застосувань, які потребують безпечного, масштабованого та гнучкого розгортання AI-агентів.

## У чому різниця між цими фреймворками?

Здається, що між цими фреймворками є багато спільного, але є ключові відмінності в їхньому дизайні, можливостях і цільових випадках використання:

- **AutoGen**: Це експериментальний фреймворк, орієнтований на передові дослідження мультиагентних систем. Найкраще підходить для експериментів і прототипування складних мультиагентних систем.
- **Semantic Kernel**: Це готова до використання бібліотека агентів для створення корпоративних агентних застосунків. Зосереджується на подієво-орієнтованих, розподілених агентних застосунках, що дозволяє використовувати кілька LLM і SLM, інструменти та одно-/мультиагентні шаблони дизайну.
- **Azure AI Agent Service**: Це платформа та служба розгортання в Azure Foundry для агентів. Вона пропонує підключення до сервісів, підтримуваних Azure, таких як Azure OpenAI, Azure AI Search, Bing Search і виконання коду.

Все ще не впевнені, який вибрати?

### Випадки використання

Давайте спробуємо допомогти, розглянувши деякі поширені випадки використання:

> Питання: Я експериментую, вивчаю та створюю прототипи агентних застосунків і хочу швидко будувати та експериментувати.
>
> Відповідь: AutoGen буде гарним вибором для цього сценарію, оскільки він зосереджується на подієво-орієнтованих, розподілених агентних застосунках і підтримує передові мультиагентні шаблони дизайну.

> Питання: Чому AutoGen краще підходить, ніж Semantic Kernel і Azure AI Agent Service, для цього випадку використання?
>
> Відповідь: AutoGen спеціально розроблений для подієво-орієнтованих, розподілених агентних застосунків, що робить його добре придатним для автоматизації завдань генерації коду та аналізу даних. Він надає необхідні інструменти та можливості для ефективного створення складних мультиагентних систем.

> Питання: Здається, Azure AI Agent Service також може підійти, адже він має інструменти для генерації коду та інше?
>
> Відповідь: Так, Azure AI Agent Service — це платформна служба для агентів із вбудованими можливостями для кількох моделей, Azure AI Search, Bing Search і Azure Functions. Це спрощує створення ваших агентів у Foundry Portal і їхнє масштабоване розгортання.

> Питання: Я все ще заплутаний, просто дайте мені один варіант.
>
> Відповідь: Чудовим вибором буде спочатку створити ваш застосунок у Semantic Kernel, а потім використовувати Azure AI Agent Service для розгортання вашого агента. Такий підхід дозволяє легко зберігати ваших агентів, використовуючи потужність Semantic Kernel для створення мультиагентних систем. Крім того, Semantic Kernel має конектор в AutoGen, що спрощує використання обох фреймворків разом.

Давайте підсумуємо ключові відмінності в таблиці:

| Фреймворк | Фокус | Основні концепції | Випадки використання |
| --- | --- | --- | --- |
| AutoGen | Подієво-орієнтовані, розподілені агентні застосунки | Агенти, Персони, Функції, Дані | Генерація коду, завдання аналізу даних |
| Semantic Kernel | Розуміння та генерація текстового контенту, схожого на людський | Агенти, Модульні компоненти, Співпраця | Розуміння природної мови, генерація контенту |
| Azure AI Agent Service | Гнучкі моделі, корпоративна безпека, Генерація коду, Виклик інструментів | Модульність, Співпраця, Оркестрація процесів | Безпечне, масштабоване та гнучке розгортання AI-агентів |

Який ідеальний випадок використання для кожного з цих фреймворків?

## Чи можу я інтегрувати свої існуючі інструменти Azure екосистеми безпосередньо, чи потрібні окремі рішення?

Відповідь — так, ви можете інтегрувати свої існуючі інструменти Azure екосистеми безпосередньо з Azure AI Agent Service, особливо тому, що він створений для безшовної роботи з іншими сервісами Azure. Наприклад, ви можете інтегрувати Bing, Azure AI Search і Azure Functions. Також є глибока інтеграція з Azure AI Foundry.

Для AutoGen і Semantic Kernel ви також можете інтегруватися з сервісами Azure, але це може вимагати виклику сервісів Azure із вашого коду. Інший спосіб інтеграції — використання Azure SDK для взаємодії з сервісами Azure із ваших агентів. Крім того, як уже згадувалося, ви можете використовувати Azure AI Agent Service як оркестратор для ваших агентів, створених в AutoGen або Semantic Kernel, що забезпечить легкий доступ до екосистеми Azure.

### Маєте більше запитань про AI Agent Frameworks?

Приєднуйтесь до [Azure AI Foundry Discord](https://aka.ms/ai-agents/discord), щоб зустрітися з іншими учнями, відвідати години консультацій і отримати відповіді на ваші запитання про AI-агентів.

## Посилання

## Попередній урок

[Вступ до AI-агентів і випадків використання агентів](../01-intro-to-ai-agents/README.md)

## Наступний урок

[Розуміння шаблонів дизайну агентів](../03-agentic-design-patterns/README.md)

---

**Відмова від відповідальності**:  
Цей документ був перекладений за допомогою сервісу автоматичного перекладу [Co-op Translator](https://github.com/Azure/co-op-translator). Хоча ми прагнемо до точності, будь ласка, майте на увазі, що автоматичні переклади можуть містити помилки або неточності. Оригінальний документ на його рідній мові слід вважати авторитетним джерелом. Для критичної інформації рекомендується професійний людський переклад. Ми не несемо відповідальності за будь-які непорозуміння або неправильні тлумачення, що виникають внаслідок використання цього перекладу.