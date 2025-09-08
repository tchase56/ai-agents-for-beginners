<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-29T21:09:36+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "bg"
}
-->
[![Изследване на рамки за AI агенти](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.bg.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(Кликнете върху изображението по-горе, за да гледате видеото на този урок)_

# Изследване на рамки за AI агенти

Рамките за AI агенти са софтуерни платформи, създадени да улеснят създаването, внедряването и управлението на AI агенти. Тези рамки предоставят на разработчиците предварително изградени компоненти, абстракции и инструменти, които опростяват разработването на сложни AI системи.

Тези рамки помагат на разработчиците да се фокусират върху уникалните аспекти на своите приложения, като предоставят стандартизирани подходи към общите предизвикателства в разработването на AI агенти. Те подобряват мащабируемостта, достъпността и ефективността при изграждането на AI системи.

## Въведение

Този урок ще обхване:

- Какво представляват рамките за AI агенти и какво позволяват на разработчиците да постигнат?
- Как екипите могат да ги използват за бързо прототипиране, итерация и подобряване на възможностите на своите агенти?
- Какви са разликите между рамките и инструментите, създадени от Microsoft, и други?
- Мога ли да интегрирам съществуващите си инструменти от екосистемата на Azure директно, или са необходими самостоятелни решения?
- Какво представлява услугата Azure AI Agents и как тя ми помага?

## Цели на обучението

Целите на този урок са да ви помогнат да разберете:

- Ролята на рамките за AI агенти в разработването на AI.
- Как да използвате рамките за AI агенти за изграждане на интелигентни агенти.
- Основните възможности, които предоставят рамките за AI агенти.
- Разликите между AutoGen, Semantic Kernel и Azure AI Agent Service.

## Какво представляват рамките за AI агенти и какво позволяват на разработчиците да правят?

Традиционните AI рамки могат да ви помогнат да интегрирате AI във вашите приложения и да ги направите по-добри по следните начини:

- **Персонализация**: AI може да анализира поведението и предпочитанията на потребителите, за да предоставя персонализирани препоръки, съдържание и преживявания.  
Пример: Стрийминг услуги като Netflix използват AI, за да предлагат филми и предавания въз основа на историята на гледане, подобрявайки ангажираността и удовлетворението на потребителите.
- **Автоматизация и ефективност**: AI може да автоматизира повтарящи се задачи, да оптимизира работните процеси и да подобрява оперативната ефективност.  
Пример: Приложения за обслужване на клиенти използват AI чатботове, за да обработват често срещани запитвания, намалявайки времето за отговор и освобождавайки човешките агенти за по-сложни въпроси.
- **Подобрено потребителско изживяване**: AI може да подобри цялостното потребителско изживяване, като предоставя интелигентни функции като разпознаване на глас, обработка на естествен език и предсказуем текст.  
Пример: Виртуални асистенти като Siri и Google Assistant използват AI, за да разбират и отговарят на гласови команди, улеснявайки взаимодействието на потребителите с техните устройства.

### Звучи страхотно, нали? Тогава защо ни е необходима рамка за AI агенти?

Рамките за AI агенти представляват нещо повече от обикновени AI рамки. Те са създадени, за да позволят създаването на интелигентни агенти, които могат да взаимодействат с потребители, други агенти и околната среда, за да постигат конкретни цели. Тези агенти могат да проявяват автономно поведение, да вземат решения и да се адаптират към променящи се условия. Нека разгледаме някои ключови възможности, които предоставят рамките за AI агенти:

- **Сътрудничество и координация между агенти**: Позволяват създаването на множество AI агенти, които могат да работят заедно, да комуникират и да координират действията си за решаване на сложни задачи.
- **Автоматизация и управление на задачи**: Осигуряват механизми за автоматизиране на многоетапни работни процеси, делегиране на задачи и динамично управление на задачи между агенти.
- **Контекстуално разбиране и адаптация**: Оборудват агентите със способността да разбират контекста, да се адаптират към променящата се среда и да вземат решения въз основа на информация в реално време.

В обобщение, агентите ви позволяват да правите повече, да издигнете автоматизацията на следващо ниво и да създавате по-интелигентни системи, които могат да се адаптират и учат от своята среда.

## Как бързо да прототипираме, итеративно подобряваме и разширяваме възможностите на агента?

Това е бързо развиваща се област, но има някои общи неща в повечето рамки за AI агенти, които могат да ви помогнат да прототипирате и итеративно подобрявате, а именно модулни компоненти, инструменти за сътрудничество и обучение в реално време. Нека разгледаме тези аспекти:

- **Използвайте модулни компоненти**: AI SDK предоставят предварително изградени компоненти като AI и Memory конектори, извикване на функции чрез естествен език или плъгини за код, шаблони за подканващи съобщения и други.
- **Възползвайте се от инструменти за сътрудничество**: Проектирайте агенти със специфични роли и задачи, което позволява тестване и усъвършенстване на съвместни работни процеси.
- **Учете в реално време**: Внедрете обратни връзки, при които агентите се учат от взаимодействия и динамично коригират поведението си.

### Използвайте модулни компоненти

SDK като Microsoft Semantic Kernel и LangChain предлагат предварително изградени компоненти като AI конектори, шаблони за подканващи съобщения и управление на паметта.

**Как екипите могат да ги използват**: Екипите могат бързо да сглобят тези компоненти, за да създадат функционален прототип, без да започват от нулата, което позволява бързо експериментиране и итерация.

**Как работи на практика**: Можете да използвате предварително изграден парсер, за да извлечете информация от потребителски вход, модул за памет за съхранение и извличане на данни и генератор на подканващи съобщения за взаимодействие с потребители, без да се налага да изграждате тези компоненти от нулата.

**Примерен код**. Нека разгледаме примери за това как можете да използвате предварително изграден AI конектор със Semantic Kernel Python и .Net, който използва автоматично извикване на функции, за да накара модела да отговаря на потребителски вход:

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

От този пример можете да видите как можете да използвате предварително изграден парсер, за да извлечете ключова информация от потребителски вход, като например произход, дестинация и дата на заявка за резервация на полет. Този модулен подход ви позволява да се фокусирате върху високото ниво на логика.

### Възползвайте се от инструменти за сътрудничество

Рамки като CrewAI, Microsoft AutoGen и Semantic Kernel улесняват създаването на множество агенти, които могат да работят заедно.

**Как екипите могат да ги използват**: Екипите могат да проектират агенти със специфични роли и задачи, което позволява тестване и усъвършенстване на съвместни работни процеси и подобряване на цялостната ефективност на системата.

**Как работи на практика**: Можете да създадете екип от агенти, където всеки агент има специализирана функция, като извличане на данни, анализ или вземане на решения. Тези агенти могат да комуникират и споделят информация, за да постигнат обща цел, като например отговаряне на потребителски въпрос или изпълнение на задача.

**Примерен код (AutoGen)**:

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

В предишния код виждате как можете да създадете задача, която включва множество агенти, работещи заедно за анализ на данни. Всеки агент изпълнява специфична функция, а задачата се изпълнява чрез координиране на агентите за постигане на желания резултат. Създавайки специализирани агенти с конкретни роли, можете да подобрите ефективността и производителността на задачите.

### Учете в реално време

Напредналите рамки предоставят възможности за разбиране на контекста и адаптация в реално време.

**Как екипите могат да ги използват**: Екипите могат да внедрят обратни връзки, при които агентите се учат от взаимодействия и динамично коригират поведението си, водейки до непрекъснато подобрение и усъвършенстване на възможностите.

**Как работи на практика**: Агенти могат да анализират обратна връзка от потребители, данни от околната среда и резултати от задачи, за да актуализират базата си от знания, да коригират алгоритмите за вземане на решения и да подобряват производителността си с времето. Този итеративен процес на учене позволява на агентите да се адаптират към променящи се условия и предпочитания на потребителите, подобрявайки цялостната ефективност на системата.

## Какви са разликите между рамките AutoGen, Semantic Kernel и Azure AI Agent Service?

Има много начини за сравнение на тези рамки, но нека разгледаме някои ключови разлики по отношение на техния дизайн, възможности и целеви случаи на употреба:

## AutoGen

AutoGen е рамка с отворен код, разработена от AI Frontiers Lab на Microsoft Research. Тя се фокусира върху събитийно-ориентирани, разпределени *агентни* приложения, позволяващи множество LLMs и SLMs, инструменти и напреднали модели за дизайн на многоагентни системи.

AutoGen е изградена около основната концепция за агенти, които са автономни единици, способни да възприемат своята среда, да вземат решения и да предприемат действия за постигане на конкретни цели. Агентите комуникират чрез асинхронни съобщения, което им позволява да работят независимо и паралелно, подобрявайки мащабируемостта и отзивчивостта на системата.

Според Wikipedia, актьорът е _основният градивен елемент на конкурентното изчисление. В отговор на съобщение, което получава, актьорът може: да взема локални решения, да създава повече актьори, да изпраща повече съобщения и да определя как да отговори на следващото получено съобщение_.

**Случаи на употреба**: Автоматизация на генерирането на код, задачи за анализ на данни и изграждане на персонализирани агенти за функции като планиране и изследвания.

Ето някои важни основни концепции на AutoGen:

- **Агенти**. Агентът е софтуерна единица, която:
  - **Комуникира чрез съобщения**, които могат да бъдат синхронни или асинхронни.
  - **Поддържа собствено състояние**, което може да бъде променено от входящи съобщения.
  - **Извършва действия** в отговор на получени съобщения или промени в състоянието си. Тези действия могат да променят състоянието на агента и да произведат външни ефекти, като актуализиране на дневници на съобщения, изпращане на нови съобщения, изпълнение на код или извършване на API повиквания.

  Ето кратък кодов фрагмент, в който създавате свой собствен агент с възможности за чат:

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

    В предишния код `MyAssistant` е създаден и наследява от `RoutedAgent`. Той има обработчик на съобщения, който отпечатва съдържанието на съобщението и след това изпраща отговор, използвайки делегата `AssistantAgent`. Особено обърнете внимание как присвояваме на `self._delegate` инстанция на `AssistantAgent`, който е предварително изграден агент, способен да обработва чат завършвания.

    Нека уведомим AutoGen за този тип агент и стартираме програмата:

    ```python
    
    # main.py
    runtime = SingleThreadedAgentRuntime()
    await MyAgent.register(runtime, "my_agent", lambda: MyAgent())

    runtime.start()  # Start processing messages in the background.
    await runtime.send_message(MyMessageType("Hello, World!"), AgentId("my_agent", "default"))
    ```  

    В предишния код агентите са регистрирани с изпълнителната среда и след това съобщение е изпратено до агента, което води до следния изход:

    ```text
    # Output from the console:
    my_agent received message: Hello, World!
    my_assistant received message: Hello, World!
    my_assistant responded: Hello! How can I assist you today?
    ```  

- **Много агенти**. AutoGen поддържа създаването на множество агенти, които могат да работят заедно за постигане на сложни задачи. Агентите могат да комуникират, да споделят информация и да координират действията си, за да решават проблеми по-ефективно. За да създадете многоагентна система, можете да дефинирате различни типове агенти със специализирани функции и роли, като извличане на данни, анализ, вземане на решения и взаимодействие с потребители. Нека видим как изглежда такова създаване:

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

    В предишния код имаме `GroupChatManager`, който е регистриран с изпълнителната среда. Този мениджър е отговорен за координирането на взаимодействията между различни типове агенти, като писатели, илюстратори, редактори и потребители.

- **Изпълнителна среда за агенти**. Рамката предоставя изпълнителна среда, която позволява комуникация между агентите, управлява техните идентичности и жизнени цикли и налага граници за сигурност и поверителност. Това означава, че можете да стартирате своите агенти в сигурна и контролирана среда, гарантирайки, че те могат да взаимодействат безопасно и ефективно. Има два интересни типа изпълнителни среди:
  - **Самостоятелна изпълнителна среда**. Това е добър избор за приложения с един процес, където всички агенти са реализирани на един и същ програмен език и работят в един и същ процес. Ето илюстрация как работи:  

    Стек на приложението

    *агентите комуникират чрез съобщения през изпълнителната среда, която управлява жизнения цикъл на агентите*

  - **Разпределена изпълнителна среда за агенти**, подходяща за многопроцесни приложения, където агентите могат да бъдат реализирани на различни програмни езици и да работят на различни машини. Ето илюстрация как работи:  

## Semantic Kernel + Рамка за агенти

Semantic Kernel е готов за предприятия AI Orchestration SDK. Той се състои от AI и памет конектори, заедно с рамка за агенти.

Нека първо разгледаме някои основни компоненти:

- **AI конектори**: Това е интерфейс с външни AI услуги и източници на данни за използване както в Python, така и в C#.

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

    Тук имате прост пример как можете да създадете ядро и да добавите услуга за чат завършване. Semantic Kernel създава връзка с външна AI услуга, в този случай Azure OpenAI Chat Completion.

- **Плъгини**: Те капсулират функции, които приложението може да използва. Има както готови плъгини, така и персонализирани, които можете да създадете. Свързана концепция е "функции за подканващи съобщения". Вместо да предоставяте естественоезикови подсказки за извикване
## Azure AI Agent Service

Azure AI Agent Service е по-ново допълнение, представено на Microsoft Ignite 2024. То позволява разработването и внедряването на AI агенти с по-гъвкави модели, като директно извикване на open-source LLMs като Llama 3, Mistral и Cohere.

Azure AI Agent Service предоставя по-силни механизми за сигурност на корпоративно ниво и методи за съхранение на данни, което го прави подходящо за корпоративни приложения.

Работи без допълнителна настройка с рамки за оркестрация на много агенти като AutoGen и Semantic Kernel.

Тази услуга в момента е в Public Preview и поддържа Python и C# за създаване на агенти.

С помощта на Semantic Kernel Python можем да създадем Azure AI Agent с потребителски дефиниран плъгин:

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

### Основни концепции

Azure AI Agent Service включва следните основни концепции:

- **Агент**. Azure AI Agent Service се интегрира с Azure AI Foundry. В рамките на AI Foundry, AI агентът действа като "умен" микросървис, който може да се използва за отговаряне на въпроси (RAG), изпълнение на действия или напълно автоматизиране на работни процеси. Това се постига чрез комбиниране на мощта на генеративните AI модели с инструменти, които му позволяват да има достъп и да взаимодейства с реални източници на данни. Ето пример за агент:

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    В този пример е създаден агент с модела `gpt-4o-mini`, име `my-agent` и инструкции `You are helpful agent`. Агентът е оборудван с инструменти и ресурси за изпълнение на задачи за интерпретация на код.

- **Тема и съобщения**. Темата е друга важна концепция. Тя представлява разговор или взаимодействие между агент и потребител. Темите могат да се използват за проследяване на напредъка на разговора, съхраняване на контекстна информация и управление на състоянието на взаимодействието. Ето пример за тема:

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

    В предходния код е създадена тема. След това съобщение е изпратено към темата. Чрез извикване на `create_and_process_run`, агентът е помолен да извърши работа върху темата. Накрая съобщенията са извлечени и записани, за да се види отговорът на агента. Съобщенията показват напредъка на разговора между потребителя и агента. Също така е важно да се разбере, че съобщенията могат да бъдат от различни типове, като текст, изображение или файл, което означава, че работата на агента е довела например до изображение или текстов отговор. Като разработчик, можете да използвате тази информация, за да обработите допълнително отговора или да го представите на потребителя.

- **Интеграция с други AI рамки**. Azure AI Agent Service може да взаимодейства с други рамки като AutoGen и Semantic Kernel, което означава, че можете да изградите част от приложението си в една от тези рамки, например използвайки Agent Service като оркестратор, или можете да изградите всичко в Agent Service.

**Приложения**: Azure AI Agent Service е предназначен за корпоративни приложения, които изискват сигурно, мащабируемо и гъвкаво внедряване на AI агенти.

## Каква е разликата между тези рамки?

Изглежда, че има много припокриване между тези рамки, но има някои ключови разлики по отношение на техния дизайн, възможности и целеви приложения:

- **AutoGen**: Е рамка за експериментиране, фокусирана върху авангардни изследвания на системи с много агенти. Това е най-доброто място за експериментиране и прототипиране на сложни системи с много агенти.
- **Semantic Kernel**: Е готова за производство библиотека за агенти за изграждане на корпоративни агентни приложения. Фокусира се върху приложения, базирани на събития, разпределени агентни приложения, позволяващи множество LLMs и SLMs, инструменти и модели за дизайн с един или много агенти.
- **Azure AI Agent Service**: Е платформа и услуга за внедряване в Azure Foundry за агенти. Тя предлага изграждане на свързаност към услуги, поддържани от Azure, като Azure OpenAI, Azure AI Search, Bing Search и изпълнение на код.

Все още не сте сигурни коя да изберете?

### Приложения

Нека се опитаме да ви помогнем, като разгледаме някои често срещани приложения:

> В: Експериментирам, уча и изграждам proof-of-concept приложения за агенти и искам да мога да изграждам и експериментирам бързо.
>

> О: AutoGen би бил добър избор за този сценарий, тъй като се фокусира върху приложения, базирани на събития, разпределени агентни приложения и поддържа усъвършенствани модели за дизайн с много агенти.

> В: Какво прави AutoGen по-добър избор от Semantic Kernel и Azure AI Agent Service за този случай?
>
> О: AutoGen е специално проектиран за приложения, базирани на събития, разпределени агентни приложения, което го прави подходящ за автоматизиране на задачи за генериране на код и анализ на данни. Той предоставя необходимите инструменти и възможности за ефективно изграждане на сложни системи с много агенти.

> В: Звучи като Azure AI Agent Service също би могъл да работи тук, той има инструменти за генериране на код и други?
>
> О: Да, Azure AI Agent Service е платформа за агенти и добавя вградени възможности за множество модели, Azure AI Search, Bing Search и Azure Functions. Той улеснява изграждането на вашите агенти в Foundry Portal и тяхното мащабно внедряване.

> В: Все още съм объркан, просто ми дайте една опция.
>
> О: Отличен избор е да изградите приложението си в Semantic Kernel първо и след това да използвате Azure AI Agent Service за внедряване на вашия агент. Този подход ви позволява лесно да запазите вашите агенти, като същевременно използвате мощта за изграждане на системи с много агенти в Semantic Kernel. Освен това Semantic Kernel има конектор в AutoGen, което улеснява използването на двете рамки заедно.

Нека обобщим ключовите разлики в таблица:

| Рамка | Фокус | Основни концепции | Приложения |
| --- | --- | --- | --- |
| AutoGen | Приложения, базирани на събития, разпределени агентни приложения | Агенти, Персони, Функции, Данни | Генериране на код, задачи за анализ на данни |
| Semantic Kernel | Разбиране и генериране на текстово съдържание, подобно на човешко | Агенти, Модулни компоненти, Сътрудничество | Разбиране на естествен език, генериране на съдържание |
| Azure AI Agent Service | Гъвкави модели, корпоративна сигурност, Генериране на код, Извикване на инструменти | Модулност, Сътрудничество, Оркестрация на процеси | Сигурно, мащабируемо и гъвкаво внедряване на AI агенти |

Какво е идеалното приложение за всяка от тези рамки?

## Мога ли да интегрирам директно съществуващите инструменти от Azure екосистемата или ми трябват самостоятелни решения?

Отговорът е да, можете да интегрирате съществуващите инструменти от Azure екосистемата директно с Azure AI Agent Service, особено защото е създаден да работи безпроблемно с други Azure услуги. Например, можете да интегрирате Bing, Azure AI Search и Azure Functions. Има и дълбока интеграция с Azure AI Foundry.

За AutoGen и Semantic Kernel също можете да интегрирате с Azure услуги, но може да се наложи да извикате Azure услугите от вашия код. Друг начин за интеграция е използването на Azure SDKs за взаимодействие с Azure услуги от вашите агенти. Освен това, както беше споменато, можете да използвате Azure AI Agent Service като оркестратор за вашите агенти, изградени в AutoGen или Semantic Kernel, което би осигурило лесен достъп до Azure екосистемата.

### Имате още въпроси относно AI Agent Frameworks?

Присъединете се към [Azure AI Foundry Discord](https://aka.ms/ai-agents/discord), за да се срещнете с други обучаващи се, да присъствате на офис часове и да получите отговори на вашите въпроси за AI агенти.

## Референции

## Предишен урок

[Въведение в AI агенти и приложения за агенти](../01-intro-to-ai-agents/README.md)

## Следващ урок

[Разбиране на модели за агентен дизайн](../03-agentic-design-patterns/README.md)

---

**Отказ от отговорност**:  
Този документ е преведен с помощта на AI услуга за превод [Co-op Translator](https://github.com/Azure/co-op-translator). Въпреки че се стремим към точност, моля, имайте предвид, че автоматизираните преводи може да съдържат грешки или неточности. Оригиналният документ на неговия роден език трябва да се счита за авторитетен източник. За критична информация се препоръчва професионален човешки превод. Ние не носим отговорност за каквито и да било недоразумения или погрешни интерпретации, произтичащи от използването на този превод.