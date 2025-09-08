<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-29T12:29:50+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "ru"
}
-->
[![Изучение фреймворков для AI-агентов](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.ru.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(Нажмите на изображение выше, чтобы посмотреть видео этого урока)_

# Изучение фреймворков для AI-агентов

Фреймворки для AI-агентов — это программные платформы, разработанные для упрощения создания, развертывания и управления AI-агентами. Эти фреймворки предоставляют разработчикам готовые компоненты, абстракции и инструменты, которые упрощают разработку сложных AI-систем.

Они помогают разработчикам сосредоточиться на уникальных аспектах их приложений, предлагая стандартизированные подходы к общим задачам разработки AI-агентов. Это повышает масштабируемость, доступность и эффективность при создании AI-систем.

## Введение

В этом уроке мы рассмотрим:

- Что такое фреймворки для AI-агентов и что они позволяют разработчикам делать?
- Как команды могут использовать их для быстрого прототипирования, итерации и улучшения возможностей своих агентов?
- Какие различия существуют между фреймворками и инструментами, созданными Microsoft, и другими?

- Можно ли интегрировать существующие инструменты экосистемы Azure напрямую или нужны отдельные решения?
- Что такое сервис Azure AI Agents и как он может помочь?

## Цели обучения

Цели этого урока — помочь вам понять:

- Роль фреймворков для AI-агентов в разработке AI.
- Как использовать фреймворки для AI-агентов для создания интеллектуальных агентов.
- Основные возможности, которые предоставляют фреймворки для AI-агентов.
- Различия между AutoGen, Semantic Kernel и Azure AI Agent Service.

## Что такое фреймворки для AI-агентов и что они позволяют разработчикам делать?

Традиционные AI-фреймворки помогают интегрировать AI в приложения и улучшать их в следующих аспектах:

- **Персонализация**: AI может анализировать поведение и предпочтения пользователей, чтобы предоставлять персонализированные рекомендации, контент и опыт.
Пример: Стриминговые сервисы, такие как Netflix, используют AI для предложения фильмов и шоу на основе истории просмотров, повышая вовлеченность и удовлетворенность пользователей.
- **Автоматизация и эффективность**: AI может автоматизировать повторяющиеся задачи, оптимизировать рабочие процессы и улучшать операционную эффективность.
Пример: Приложения для обслуживания клиентов используют чат-ботов на основе AI для обработки стандартных запросов, сокращая время ответа и освобождая человеческих агентов для более сложных задач.
- **Улучшение пользовательского опыта**: AI может улучшить общий пользовательский опыт, предоставляя интеллектуальные функции, такие как распознавание голоса, обработка естественного языка и предиктивный текст.
Пример: Виртуальные помощники, такие как Siri и Google Assistant, используют AI для понимания и выполнения голосовых команд, упрощая взаимодействие пользователей с устройствами.

### Звучит здорово, правда? Так зачем нам нужны фреймворки для AI-агентов?

Фреймворки для AI-агентов представляют собой нечто большее, чем просто AI-фреймворки. Они разработаны для создания интеллектуальных агентов, которые могут взаимодействовать с пользователями, другими агентами и окружающей средой для достижения конкретных целей. Эти агенты могут демонстрировать автономное поведение, принимать решения и адаптироваться к изменяющимся условиям. Давайте рассмотрим ключевые возможности, которые предоставляют фреймворки для AI-агентов:

- **Сотрудничество и координация агентов**: Позволяют создавать несколько AI-агентов, которые могут работать вместе, общаться и координировать действия для решения сложных задач.
- **Автоматизация и управление задачами**: Предоставляют механизмы для автоматизации многоэтапных рабочих процессов, делегирования задач и динамического управления задачами между агентами.
- **Контекстуальное понимание и адаптация**: Оснащают агентов способностью понимать контекст, адаптироваться к изменяющимся условиям и принимать решения на основе информации в реальном времени.

Таким образом, агенты позволяют делать больше, выводить автоматизацию на новый уровень, создавать более интеллектуальные системы, которые могут адаптироваться и учиться на основе окружающей среды.

## Как быстро прототипировать, итеративно улучшать и развивать возможности агентов?

Это быстро развивающаяся область, но есть несколько общих аспектов, которые можно найти в большинстве фреймворков для AI-агентов и которые помогут вам быстро прототипировать и итеративно улучшать, а именно модульные компоненты, инструменты для совместной работы и обучение в реальном времени. Давайте углубимся в эти аспекты:

- **Используйте модульные компоненты**: SDK для AI предлагают готовые компоненты, такие как коннекторы для AI и памяти, вызов функций с использованием естественного языка или плагинов кода, шаблоны подсказок и многое другое.
- **Используйте инструменты для совместной работы**: Разрабатывайте агентов с конкретными ролями и задачами, что позволяет тестировать и совершенствовать совместные рабочие процессы.
- **Обучение в реальном времени**: Реализуйте циклы обратной связи, где агенты учатся на взаимодействиях и динамически корректируют свое поведение.

### Используйте модульные компоненты

SDK, такие как Microsoft Semantic Kernel и LangChain, предлагают готовые компоненты, такие как коннекторы для AI, шаблоны подсказок и управление памятью.

**Как команды могут использовать это**: Команды могут быстро собрать эти компоненты, чтобы создать функциональный прототип без необходимости начинать с нуля, что позволяет быстро экспериментировать и проводить итерации.

**Как это работает на практике**: Вы можете использовать готовый парсер для извлечения информации из пользовательского ввода, модуль памяти для хранения и извлечения данных, а также генератор подсказок для взаимодействия с пользователями — все это без необходимости создавать эти компоненты с нуля.

**Пример кода**. Давайте посмотрим примеры того, как можно использовать готовый AI-коннектор с Semantic Kernel Python и .Net, который использует автоматический вызов функций для ответа модели на пользовательский ввод:

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

На этом примере видно, как можно использовать готовый парсер для извлечения ключевой информации из пользовательского ввода, например, места отправления, назначения и даты запроса на бронирование рейса. Такой модульный подход позволяет сосредоточиться на логике высокого уровня.

### Используйте инструменты для совместной работы

Фреймворки, такие как CrewAI, Microsoft AutoGen и Semantic Kernel, облегчают создание нескольких агентов, которые могут работать вместе.

**Как команды могут использовать это**: Команды могут разрабатывать агентов с конкретными ролями и задачами, что позволяет тестировать и совершенствовать совместные рабочие процессы и повышать общую эффективность системы.

**Как это работает на практике**: Вы можете создать команду агентов, где каждый агент выполняет специализированную функцию, например, извлечение данных, анализ или принятие решений. Эти агенты могут общаться и обмениваться информацией для достижения общей цели, например, ответа на запрос пользователя или выполнения задачи.

**Пример кода (AutoGen)**:

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

На предыдущем примере видно, как можно создать задачу, включающую несколько агентов, работающих вместе для анализа данных. Каждый агент выполняет определенную функцию, а задача выполняется путем координации агентов для достижения желаемого результата. Создавая специализированных агентов с определенными ролями, можно улучшить эффективность и производительность задач.

### Обучение в реальном времени

Продвинутые фреймворки предоставляют возможности для понимания контекста и адаптации в реальном времени.

**Как команды могут использовать это**: Команды могут реализовать циклы обратной связи, где агенты учатся на взаимодействиях и динамически корректируют свое поведение, что приводит к постоянному улучшению и совершенствованию возможностей.

**Как это работает на практике**: Агенты могут анализировать отзывы пользователей, данные окружающей среды и результаты задач, чтобы обновлять свою базу знаний, корректировать алгоритмы принятия решений и улучшать производительность со временем. Этот итеративный процесс обучения позволяет агентам адаптироваться к изменяющимся условиям и предпочтениям пользователей, повышая общую эффективность системы.

## Какие различия между фреймворками AutoGen, Semantic Kernel и Azure AI Agent Service?

Существует множество способов сравнения этих фреймворков, но давайте рассмотрим ключевые различия с точки зрения их дизайна, возможностей и целевых сценариев использования:

## AutoGen

AutoGen — это фреймворк с открытым исходным кодом, разработанный AI Frontiers Lab Microsoft Research. Он ориентирован на событийно-управляемые, распределенные *агентные* приложения, позволяя использовать несколько LLM и SLM, инструменты и продвинутые многопользовательские агентные шаблоны.

AutoGen построен вокруг основной концепции агентов, которые являются автономными сущностями, способными воспринимать окружающую среду, принимать решения и выполнять действия для достижения конкретных целей. Агенты общаются через асинхронные сообщения, что позволяет им работать независимо и параллельно, повышая масштабируемость и отзывчивость системы.

Согласно Википедии, актор — это _основной строительный блок параллельных вычислений. В ответ на полученное сообщение актор может: принимать локальные решения, создавать новых акторов, отправлять сообщения и определять, как реагировать на следующее полученное сообщение_.

**Сценарии использования**: Автоматизация генерации кода, задачи анализа данных и создание пользовательских агентов для функций планирования и исследований.

Вот некоторые важные основные концепции AutoGen:

- **Агенты**. Агент — это программная сущность, которая:
  - **Общается через сообщения**, которые могут быть синхронными или асинхронными.
  - **Поддерживает собственное состояние**, которое может изменяться входящими сообщениями.
  - **Выполняет действия** в ответ на полученные сообщения или изменения своего состояния. Эти действия могут изменять состояние агента и производить внешние эффекты, такие как обновление журналов сообщений, отправка новых сообщений, выполнение кода или вызов API.

  Вот короткий пример кода, в котором создается собственный агент с функциями чата:

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

    В предыдущем коде создан `MyAssistant`, который наследуется от `RoutedAgent`. У него есть обработчик сообщений, который выводит содержимое сообщения, а затем отправляет ответ с помощью делегата `AssistantAgent`. Особенно обратите внимание, как мы назначаем `self._delegate` экземпляр `AssistantAgent`, который является готовым агентом, способным обрабатывать завершения чата.

    Давайте сообщим AutoGen об этом типе агента и запустим программу:

    ```python
    
    # main.py
    runtime = SingleThreadedAgentRuntime()
    await MyAgent.register(runtime, "my_agent", lambda: MyAgent())

    runtime.start()  # Start processing messages in the background.
    await runtime.send_message(MyMessageType("Hello, World!"), AgentId("my_agent", "default"))
    ```

    В предыдущем коде агенты регистрируются в среде выполнения, а затем сообщение отправляется агенту, что приводит к следующему выводу:

    ```text
    # Output from the console:
    my_agent received message: Hello, World!
    my_assistant received message: Hello, World!
    my_assistant responded: Hello! How can I assist you today?
    ```

- **Множественные агенты**. AutoGen поддерживает создание нескольких агентов, которые могут работать вместе для выполнения сложных задач. Агенты могут общаться, обмениваться информацией и координировать свои действия для более эффективного решения проблем. Чтобы создать систему с несколькими агентами, вы можете определить различные типы агентов с специализированными функциями и ролями, такими как извлечение данных, анализ, принятие решений и взаимодействие с пользователем. Давайте посмотрим, как выглядит такое создание:

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

    В предыдущем коде у нас есть `GroupChatManager`, который зарегистрирован в среде выполнения. Этот менеджер отвечает за координацию взаимодействий между различными типами агентов, такими как писатели, иллюстраторы, редакторы и пользователи.

- **Среда выполнения агентов**. Фреймворк предоставляет среду выполнения, которая позволяет агентам общаться, управляет их идентичностью и жизненным циклом, а также обеспечивает соблюдение границ безопасности и конфиденциальности. Это означает, что вы можете запускать своих агентов в безопасной и контролируемой среде, гарантируя, что они могут взаимодействовать безопасно и эффективно. Существует два интересных типа среды выполнения:
  - **Автономная среда выполнения**. Это хороший выбор для приложений с одним процессом, где все агенты реализованы на одном языке программирования и работают в одном процессе. Вот иллюстрация того, как это работает:

    Стек приложения

    *агенты общаются через сообщения через среду выполнения, а среда выполнения управляет жизненным циклом агентов*

  - **Распределенная среда выполнения агентов**, подходит для многопроцессных приложений, где агенты могут быть реализованы на разных языках программирования и работать на разных машинах. Вот иллюстрация того, как это работает:

## Semantic Kernel + Agent Framework

Semantic Kernel — это готовый для использования в корпоративной среде SDK для оркестрации AI. Он состоит из коннекторов для AI и памяти, а также фреймворка для агентов.

Сначала рассмотрим основные компоненты:

- **Коннекторы для AI**: Это интерфейс с внешними AI-сервисами и источниками данных для использования как в Python, так и в C#.

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

    Вот простой пример того, как можно создать ядро и добавить сервис завершения чата. Semantic Kernel создает соединение с внешним AI-сервисом, в данном случае Azure OpenAI Chat Completion.

- **Плагины**: Они инкапсулируют функции, которые приложение может использовать. Существуют как готовые плагины, так и пользовательские, которые вы можете создать. Связанная концепция — "функции подсказок". Вместо предоставления естественно-языковых подсказок для вызова функции, вы транслируете определенные функции модели. На основе текущего контекста чата модель может выбрать вызов одной из этих функций для выполнения запроса или вопроса. Вот пример:

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

    Здесь сначала создается шаблон подсказки `skPrompt`, который оставляет место для ввода текста пользователем, `$userInput`. Затем создается функция ядра `SummarizeText`, которая импортируется в ядро с именем плагина `SemanticFunctions`. Обратите внимание на имя функции, которое помогает Semantic Kernel понять, что делает функция и когда она должна быть вызвана.

- **Нативные функции**: Также существуют нативные функции, которые фреймворк может вызывать напрямую для выполнения задачи. Вот пример такой функции, извлекающей содержимое из файла:

    ```csharp
    public class NativeFunctions {

        [SKFunction, Description("Retrieve content from local file")]
        public async Task<string> RetrieveLocalFile(string fileName, int maxSize = 5000)
        {
            string content = await File.ReadAllTextAsync(fileName);
            if (content.Length <= maxSize) return content;
            return content.Substring(0, maxSize);
        }
    }
    
    //Import native function
    string plugInName = "NativeFunction";
    string functionName = "RetrieveLocalFile";

   //To add the functions to a kernel use the following function
    kernel.ImportPluginFromType<NativeFunctions>();

    ```

- **Память**: Абстрагирует и упрощает управление контекстом для AI-приложений. Идея памяти заключается в том, что это информация, которую LLM должен знать. Вы можете хранить эту информацию в векторном хранилище, которое в итоге становится базой данных в памяти или векторной базой данных или аналогичным. Вот пример очень упрощенного сценария, где *факты* добавляются в память:

    ```csharp
    var facts = new Dictionary<string,string>();
    facts.Add(
        "Azure Machine Learning; https://learn.microsoft.com/azure/machine-learning/",
        @"Azure Machine Learning is a cloud service for accelerating and
        managing the machine learning project lifecycle. Machine learning professionals,
        data scientists, and engineers can use it in their day-to-day workflows"
    );
    
    facts.Add(
        "Azure SQL Service; https://learn.microsoft.com/azure/azure-sql/",
        @"Azure SQL is a family of managed, secure, and intelligent products
        that use the SQL Server database engine in the Azure cloud."
    );
    
    string memoryCollectionName = "SummarizedAzureDocs";
    
    foreach (var fact in facts) {
        await memoryBuilder.SaveReferenceAsync(
            collection: memoryCollectionName,
            description: fact.Key.Split(";")[1].Trim(),
            text: fact.Value,
            externalId: fact.Key.Split(";")[2].Trim(),
            externalSourceName: "Azure Documentation"
        );
    }
    ```

    Эти факты затем сохраняются в коллекции памяти `SummarizedAzureDocs`. Это очень упрощенный пример, но вы можете увидеть, как можно хранить информацию в памяти для использования LLM.
Итак, это основы фреймворка Semantic Kernel, а что насчет Agent Framework?

## Azure AI Agent Service

Azure AI Agent Service — это более недавнее дополнение, представленное на Microsoft Ignite 2024. Оно позволяет разрабатывать и развертывать AI-агентов с более гибкими моделями, такими как прямой вызов открытых LLM, например, Llama 3, Mistral и Cohere.

Azure AI Agent Service предоставляет более надежные механизмы безопасности для предприятий и методы хранения данных, что делает его подходящим для корпоративных приложений.

Он работает "из коробки" с фреймворками оркестрации мультиагентов, такими как AutoGen и Semantic Kernel.

Этот сервис в настоящее время находится в стадии публичного предварительного просмотра и поддерживает Python и C# для создания агентов.

Используя Semantic Kernel Python, мы можем создать Azure AI Agent с пользовательским плагином:

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

### Основные концепции

Azure AI Agent Service включает следующие основные концепции:

- **Агент**. Azure AI Agent Service интегрируется с Azure AI Foundry. В рамках AI Foundry AI-агент действует как "умный" микросервис, который можно использовать для ответа на вопросы (RAG), выполнения действий или полной автоматизации рабочих процессов. Это достигается благодаря сочетанию возможностей генеративных AI-моделей с инструментами, которые позволяют получать доступ и взаимодействовать с реальными источниками данных. Вот пример агента:

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    В этом примере агент создается с моделью `gpt-4o-mini`, именем `my-agent` и инструкциями `You are helpful agent`. Агент оснащен инструментами и ресурсами для выполнения задач интерпретации кода.

- **Поток и сообщения**. Поток — это еще одна важная концепция. Он представляет собой разговор или взаимодействие между агентом и пользователем. Потоки можно использовать для отслеживания прогресса разговора, хранения информации о контексте и управления состоянием взаимодействия. Вот пример потока:

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

    В приведенном выше коде создается поток. Затем в поток отправляется сообщение. Вызвав `create_and_process_run`, агенту предлагается выполнить работу в потоке. Наконец, сообщения извлекаются и записываются, чтобы увидеть ответ агента. Сообщения показывают прогресс разговора между пользователем и агентом. Также важно понимать, что сообщения могут быть разных типов, например текст, изображение или файл, которые являются результатом работы агента, например, изображение или текстовый ответ. Как разработчик, вы можете использовать эту информацию для дальнейшей обработки ответа или его представления пользователю.

- **Интеграция с другими AI-фреймворками**. Сервис Azure AI Agent может взаимодействовать с другими фреймворками, такими как AutoGen и Semantic Kernel, что означает, что вы можете построить часть своего приложения в одном из этих фреймворков, а, например, использовать Agent Service как оркестратор или построить все приложение в Agent Service.

**Сценарии использования**: Azure AI Agent Service предназначен для корпоративных приложений, требующих безопасного, масштабируемого и гибкого развертывания AI-агентов.

## В чем разница между этими фреймворками?

Кажется, что между этими фреймворками есть много общего, но существуют ключевые различия в их дизайне, возможностях и целевых сценариях использования:

- **AutoGen**: Это экспериментальный фреймворк, ориентированный на передовые исследования мультиагентных систем. Это лучшее место для экспериментов и прототипирования сложных мультиагентных систем.
- **Semantic Kernel**: Это готовая к производству библиотека агентов для создания корпоративных агентных приложений. Ориентирован на событийно-управляемые, распределенные агентные приложения, поддерживающие несколько LLM и SLM, инструменты и шаблоны проектирования для одного/нескольких агентов.
- **Azure AI Agent Service**: Это платформа и сервис развертывания в Azure Foundry для агентов. Предлагает подключение к сервисам, поддерживаемым Azure, таким как Azure OpenAI, Azure AI Search, Bing Search и выполнение кода.

Все еще не уверены, что выбрать?

### Сценарии использования

Давайте попробуем помочь вам, рассмотрев несколько распространенных сценариев:

> В: Я экспериментирую, учусь и создаю приложения-агенты в виде концептуальных доказательств, и хочу быстро строить и экспериментировать.

> О: AutoGen будет хорошим выбором для этого сценария, так как он ориентирован на событийно-управляемые, распределенные агентные приложения и поддерживает продвинутые шаблоны проектирования мультиагентов.

> В: Что делает AutoGen лучшим выбором, чем Semantic Kernel и Azure AI Agent Service для этого сценария?

> О: AutoGen специально разработан для событийно-управляемых, распределенных агентных приложений, что делает его хорошо подходящим для автоматизации задач генерации кода и анализа данных. Он предоставляет необходимые инструменты и возможности для эффективного создания сложных мультиагентных систем.

> В: Звучит так, будто Azure AI Agent Service тоже может подойти, ведь у него есть инструменты для генерации кода и многое другое?

> О: Да, Azure AI Agent Service — это платформенный сервис для агентов, который добавляет встроенные возможности для нескольких моделей, Azure AI Search, Bing Search и Azure Functions. Это упрощает создание агентов в Foundry Portal и их масштабное развертывание.

> В: Я все еще запутан, просто дайте мне один вариант.

> О: Отличным выбором будет сначала построить ваше приложение в Semantic Kernel, а затем использовать Azure AI Agent Service для развертывания вашего агента. Такой подход позволяет легко сохранять ваших агентов, одновременно используя возможности для создания мультиагентных систем в Semantic Kernel. Кроме того, в Semantic Kernel есть коннектор в AutoGen, что упрощает использование обоих фреймворков вместе.

Давайте подытожим ключевые различия в таблице:

| Фреймворк | Фокус | Основные концепции | Сценарии использования |
| --- | --- | --- | --- |
| AutoGen | Событийно-управляемые, распределенные агентные приложения | Агенты, Персоны, Функции, Данные | Генерация кода, задачи анализа данных |
| Semantic Kernel | Понимание и генерация текста, похожего на человеческий | Агенты, Модульные компоненты, Сотрудничество | Понимание естественного языка, генерация контента |
| Azure AI Agent Service | Гибкие модели, безопасность для предприятий, Генерация кода, Вызов инструментов | Модульность, Сотрудничество, Оркестрация процессов | Безопасное, масштабируемое и гибкое развертывание AI-агентов |

Какой идеальный сценарий использования для каждого из этих фреймворков?

## Могу ли я интегрировать свои существующие инструменты экосистемы Azure напрямую или мне нужны автономные решения?

Ответ — да, вы можете интегрировать свои существующие инструменты экосистемы Azure напрямую, особенно с Azure AI Agent Service, так как он был создан для работы с другими сервисами Azure. Например, вы можете интегрировать Bing, Azure AI Search и Azure Functions. Также существует глубокая интеграция с Azure AI Foundry.

Для AutoGen и Semantic Kernel вы также можете интегрировать с сервисами Azure, но это может потребовать вызова сервисов Azure из вашего кода. Другой способ интеграции — использование SDK Azure для взаимодействия с сервисами Azure из ваших агентов. Кроме того, как уже упоминалось, вы можете использовать Azure AI Agent Service как оркестратор для ваших агентов, созданных в AutoGen или Semantic Kernel, что обеспечит легкий доступ к экосистеме Azure.

### Остались вопросы о фреймворках AI-агентов?

Присоединяйтесь к [Azure AI Foundry Discord](https://aka.ms/ai-agents/discord), чтобы встретиться с другими учащимися, посетить офисные часы и получить ответы на свои вопросы о AI-агентах.

## Ссылки

## Предыдущий урок

[Введение в AI-агентов и сценарии их использования](../01-intro-to-ai-agents/README.md)

## Следующий урок

[Понимание шаблонов проектирования агентов](../03-agentic-design-patterns/README.md)

---

**Отказ от ответственности**:  
Этот документ был переведен с помощью сервиса автоматического перевода [Co-op Translator](https://github.com/Azure/co-op-translator). Несмотря на наши усилия обеспечить точность, автоматические переводы могут содержать ошибки или неточности. Оригинальный документ на его исходном языке следует считать авторитетным источником. Для получения критически важной информации рекомендуется профессиональный перевод человеком. Мы не несем ответственности за любые недоразумения или неправильные интерпретации, возникшие в результате использования данного перевода.