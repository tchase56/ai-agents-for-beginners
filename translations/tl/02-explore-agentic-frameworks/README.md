<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-29T09:51:22+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "tl"
}
-->
[![Exploring AI Agent Frameworks](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.tl.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(I-click ang imahe sa itaas para mapanood ang video ng araling ito)_

# Tuklasin ang AI Agent Frameworks

Ang AI agent frameworks ay mga software platform na idinisenyo upang gawing mas madali ang paglikha, pag-deploy, at pamamahala ng mga AI agents. Ang mga framework na ito ay nagbibigay sa mga developer ng mga pre-built na bahagi, abstractions, at tools na nagpapabilis sa pagbuo ng mga kumplikadong AI system.

Ang mga framework na ito ay tumutulong sa mga developer na mag-focus sa natatanging aspeto ng kanilang mga aplikasyon sa pamamagitan ng pagbibigay ng standardized na mga solusyon sa mga karaniwang hamon sa pag-develop ng AI agents. Pinapahusay nito ang scalability, accessibility, at efficiency sa pagbuo ng AI systems.

## Panimula

Ang araling ito ay tatalakay sa:

- Ano ang AI Agent Frameworks at ano ang kayang gawin ng mga developer gamit ang mga ito?
- Paano magagamit ng mga team ang mga ito upang mabilis na mag-prototype, mag-iterate, at mapabuti ang kakayahan ng kanilang agent?
- Ano ang mga pagkakaiba sa pagitan ng mga framework at tools na ginawa ng Microsoft, at iba pa?
- Maaari bang direktang i-integrate ang mga kasalukuyang tools ng Azure ecosystem, o kailangan ng standalone na solusyon?
- Ano ang Azure AI Agents service at paano ito makakatulong sa akin?

## Mga Layunin sa Pag-aaral

Ang mga layunin ng araling ito ay upang matulungan kang maunawaan:

- Ang papel ng AI Agent Frameworks sa pag-develop ng AI.
- Paano gamitin ang AI Agent Frameworks upang makabuo ng mga intelligent agents.
- Mga pangunahing kakayahan na pinapagana ng AI Agent Frameworks.
- Ang mga pagkakaiba sa pagitan ng AutoGen, Semantic Kernel, at Azure AI Agent Service.

## Ano ang AI Agent Frameworks at ano ang kayang gawin ng mga developer gamit ang mga ito?

Ang tradisyunal na AI Frameworks ay makakatulong sa iyo na i-integrate ang AI sa iyong mga app at gawing mas mahusay ang mga ito sa mga sumusunod na paraan:

- **Personalization**: Ang AI ay maaaring mag-analyze ng user behavior at preferences upang magbigay ng personalized na rekomendasyon, content, at karanasan.
Halimbawa: Ang mga streaming service tulad ng Netflix ay gumagamit ng AI upang magmungkahi ng mga pelikula at palabas batay sa viewing history, na nagpapataas ng user engagement at satisfaction.
- **Automation at Efficiency**: Ang AI ay maaaring mag-automate ng mga paulit-ulit na gawain, mag-streamline ng workflows, at magpabuti ng operational efficiency.
Halimbawa: Ang mga customer service app ay gumagamit ng AI-powered chatbots upang sagutin ang mga karaniwang tanong, na nagpapababa ng response times at nagbibigay ng mas maraming oras sa mga human agents para sa mas kumplikadong isyu.
- **Enhanced User Experience**: Ang AI ay maaaring magpabuti ng kabuuang user experience sa pamamagitan ng pagbibigay ng mga intelligent na feature tulad ng voice recognition, natural language processing, at predictive text.
Halimbawa: Ang mga virtual assistant tulad ng Siri at Google Assistant ay gumagamit ng AI upang maunawaan at tumugon sa mga voice command, na nagpapadali sa pakikipag-ugnayan ng mga user sa kanilang mga device.

### Mukhang maganda, di ba? Kaya bakit kailangan natin ang AI Agent Framework?

Ang AI Agent frameworks ay higit pa sa tradisyunal na AI frameworks. Ang mga ito ay idinisenyo upang paganahin ang paglikha ng mga intelligent agents na maaaring makipag-ugnayan sa mga user, iba pang agents, at sa kapaligiran upang makamit ang mga tiyak na layunin. Ang mga agents na ito ay maaaring magpakita ng autonomous na pag-uugali, gumawa ng desisyon, at mag-adapt sa mga nagbabagong kondisyon. Tingnan natin ang ilang pangunahing kakayahan na pinapagana ng AI Agent Frameworks:

- **Agent Collaboration at Coordination**: Pinapagana ang paglikha ng maraming AI agents na maaaring magtulungan, mag-communicate, at mag-coordinate upang malutas ang mga kumplikadong gawain.
- **Task Automation at Management**: Nagbibigay ng mekanismo para sa pag-automate ng multi-step workflows, task delegation, at dynamic task management sa pagitan ng mga agents.
- **Contextual Understanding at Adaptation**: Nilalapatan ang mga agents ng kakayahang maunawaan ang konteksto, mag-adapt sa mga nagbabagong kapaligiran, at gumawa ng desisyon batay sa real-time na impormasyon.

Sa kabuuan, ang mga agents ay nagbibigay-daan sa iyo na gumawa ng higit pa, upang dalhin ang automation sa mas mataas na antas, at lumikha ng mas intelligent na mga sistema na maaaring mag-adapt at matuto mula sa kanilang kapaligiran.

## Paano mabilis na mag-prototype, mag-iterate, at mapabuti ang kakayahan ng agent?

Ito ay isang mabilis na umuunlad na landscape, ngunit may ilang mga bagay na karaniwan sa karamihan ng AI Agent Frameworks na makakatulong sa iyo na mabilis na mag-prototype at mag-iterate, tulad ng modular components, collaborative tools, at real-time learning. Tingnan natin ang mga ito:

- **Gamitin ang Modular Components**: Ang AI SDKs ay nag-aalok ng mga pre-built na bahagi tulad ng AI at Memory connectors, function calling gamit ang natural language o code plugins, prompt templates, at iba pa.
- **Gamitin ang Collaborative Tools**: Magdisenyo ng mga agents na may partikular na mga tungkulin at gawain, na nagbibigay-daan sa kanila na subukan at pagbutihin ang collaborative workflows.
- **Matuto sa Real-Time**: Magpatupad ng feedback loops kung saan natututo ang mga agents mula sa mga interaksyon at ina-adjust ang kanilang pag-uugali nang dynamic.

### Gamitin ang Modular Components

Ang mga SDK tulad ng Microsoft Semantic Kernel at LangChain ay nag-aalok ng mga pre-built na bahagi tulad ng AI connectors, prompt templates, at memory management.

**Paano magagamit ng mga team ang mga ito**: Ang mga team ay maaaring mabilis na mag-assemble ng mga bahaging ito upang makabuo ng functional prototype nang hindi nagsisimula mula sa simula, na nagbibigay-daan sa mabilis na eksperimento at iteration.

**Paano ito gumagana sa praktika**: Maaari kang gumamit ng pre-built parser upang kunin ang impormasyon mula sa user input, isang memory module upang mag-imbak at mag-retrieve ng data, at isang prompt generator upang makipag-ugnayan sa mga user, lahat nang hindi kailangang buuin ang mga bahaging ito mula sa simula.

**Halimbawa ng code**. Tingnan natin ang mga halimbawa kung paano mo magagamit ang pre-built AI Connector gamit ang Semantic Kernel Python at .Net na gumagamit ng auto-function calling upang tumugon ang model sa user input:

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

Makikita mo mula sa halimbawang ito kung paano mo magagamit ang pre-built parser upang kunin ang mahalagang impormasyon mula sa user input, tulad ng origin, destination, at petsa ng flight booking request. Ang modular na approach na ito ay nagbibigay-daan sa iyo na mag-focus sa high-level logic.

### Gamitin ang Collaborative Tools

Ang mga framework tulad ng CrewAI, Microsoft AutoGen, at Semantic Kernel ay nagpapadali sa paglikha ng maraming agents na maaaring magtulungan.

**Paano magagamit ng mga team ang mga ito**: Ang mga team ay maaaring magdisenyo ng mga agents na may partikular na mga tungkulin at gawain, na nagbibigay-daan sa kanila na subukan at pagbutihin ang collaborative workflows at mapabuti ang kabuuang system efficiency.

**Paano ito gumagana sa praktika**: Maaari kang lumikha ng isang team ng agents kung saan ang bawat agent ay may espesyal na tungkulin, tulad ng data retrieval, analysis, o decision-making. Ang mga agents na ito ay maaaring mag-communicate at magbahagi ng impormasyon upang makamit ang isang karaniwang layunin, tulad ng pagsagot sa user query o pagkompleto ng isang gawain.

**Halimbawa ng code (AutoGen)**:

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

Makikita mo sa nakaraang code kung paano mo maaaring lumikha ng isang gawain na kinabibilangan ng maraming agents na nagtutulungan upang mag-analyze ng data. Ang bawat agent ay gumaganap ng partikular na tungkulin, at ang gawain ay isinasagawa sa pamamagitan ng pag-coordinate ng mga agents upang makamit ang nais na resulta. Sa pamamagitan ng paglikha ng mga dedikadong agents na may espesyal na tungkulin, maaari mong mapabuti ang task efficiency at performance.

### Matuto sa Real-Time

Ang mga advanced na framework ay nagbibigay ng kakayahan para sa real-time na pag-unawa sa konteksto at pag-adapt.

**Paano magagamit ng mga team ang mga ito**: Ang mga team ay maaaring magpatupad ng feedback loops kung saan natututo ang mga agents mula sa mga interaksyon at ina-adjust ang kanilang pag-uugali nang dynamic, na nagreresulta sa patuloy na pagpapabuti at refinement ng kakayahan.

**Paano ito gumagana sa praktika**: Ang mga agents ay maaaring mag-analyze ng user feedback, environmental data, at task outcomes upang i-update ang kanilang knowledge base, i-adjust ang decision-making algorithms, at mapabuti ang performance sa paglipas ng panahon. Ang iterative learning process na ito ay nagbibigay-daan sa mga agents na mag-adapt sa mga nagbabagong kondisyon at user preferences, na nagpapahusay sa kabuuang system effectiveness.

## Ano ang mga pagkakaiba sa pagitan ng mga framework AutoGen, Semantic Kernel, at Azure AI Agent Service?

Maraming paraan upang ikumpara ang mga framework na ito, ngunit tingnan natin ang ilang pangunahing pagkakaiba sa kanilang disenyo, kakayahan, at target na use cases:

## AutoGen

Ang AutoGen ay isang open-source framework na binuo ng Microsoft Research's AI Frontiers Lab. Nakatuon ito sa event-driven, distributed *agentic* applications, na nagpapagana ng maraming LLMs at SLMs, tools, at advanced multi-agent design patterns.

Ang AutoGen ay binuo sa paligid ng pangunahing konsepto ng agents, na mga autonomous na entity na maaaring makaramdam ng kanilang kapaligiran, gumawa ng desisyon, at kumilos upang makamit ang mga tiyak na layunin. Ang mga agents ay nagko-communicate sa pamamagitan ng asynchronous messages, na nagbibigay-daan sa kanila na magtrabaho nang independyente at parallel, na nagpapahusay sa system scalability at responsiveness.

Ayon sa Wikipedia, ang isang actor ay _ang pangunahing building block ng concurrent computation. Sa pagtugon sa isang mensahe na natanggap, ang isang actor ay maaaring: gumawa ng lokal na desisyon, lumikha ng mas maraming actors, magpadala ng mas maraming mensahe, at tukuyin kung paano tumugon sa susunod na mensahe na natanggap_.

**Use Cases**: Pag-automate ng code generation, data analysis tasks, at pagbuo ng custom agents para sa planning at research functions.

Narito ang ilang mahalagang core concepts ng AutoGen:

- **Agents**. Ang isang agent ay isang software entity na:
  - **Nagko-communicate sa pamamagitan ng mga mensahe**, maaaring synchronous o asynchronous ang mga mensaheng ito.
  - **Nagpapanatili ng sariling estado**, na maaaring mabago ng mga natanggap na mensahe.
  - **Gumagawa ng mga aksyon** bilang tugon sa mga natanggap na mensahe o pagbabago sa estado nito. Ang mga aksyon na ito ay maaaring magbago ng estado ng agent at magdulot ng external effects, tulad ng pag-update ng message logs, pagpapadala ng bagong mensahe, pag-execute ng code, o paggawa ng API calls.

Narito ang isang maikling code snippet kung saan maaari kang lumikha ng sarili mong agent na may Chat capabilities:

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

Sa nakaraang code, ang `MyAssistant` ay nilikha at nagmana mula sa `RoutedAgent`. Mayroon itong message handler na nagpi-print ng content ng mensahe at pagkatapos ay nagpapadala ng tugon gamit ang `AssistantAgent` delegate. Lalo na tandaan kung paano natin ina-assign sa `self._delegate` ang isang instance ng `AssistantAgent` na isang pre-built agent na maaaring mag-handle ng chat completions.

Ipaalam natin sa AutoGen ang tungkol sa ganitong uri ng agent at simulan ang programa:

```python
    
    # main.py
    runtime = SingleThreadedAgentRuntime()
    await MyAgent.register(runtime, "my_agent", lambda: MyAgent())

    runtime.start()  # Start processing messages in the background.
    await runtime.send_message(MyMessageType("Hello, World!"), AgentId("my_agent", "default"))
    ```

Sa nakaraang code, ang mga agents ay nairehistro sa runtime at pagkatapos ay isang mensahe ang ipinadala sa agent na nagresulta sa sumusunod na output:

```text
    # Output from the console:
    my_agent received message: Hello, World!
    my_assistant received message: Hello, World!
    my_assistant responded: Hello! How can I assist you today?
    ```

- **Multi agents**. Sinusuportahan ng AutoGen ang paglikha ng maraming agents na maaaring magtulungan upang makamit ang mga kumplikadong gawain. Ang mga agents ay maaaring mag-communicate, magbahagi ng impormasyon, at mag-coordinate ng kanilang mga aksyon upang mas mabilis na malutas ang mga problema. Upang lumikha ng isang multi-agent system, maaari kang mag-defina ng iba't ibang uri ng agents na may espesyal na tungkulin at papel, tulad ng data retrieval, analysis, decision-making, at user interaction. Tingnan natin kung paano ang ganitong paglikha upang magkaroon tayo ng ideya:

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

Sa nakaraang code, mayroon tayong `GroupChatManager` na nairehistro sa runtime. Ang manager na ito ang responsable sa pag-coordinate ng mga interaksyon sa pagitan ng iba't ibang uri ng agents, tulad ng writers, illustrators, editors, at users.

- **Agent Runtime**. Ang framework ay nagbibigay ng runtime environment, na nagpapagana ng komunikasyon sa pagitan ng mga agents, nagma-manage ng kanilang identities at lifecycles, at nagpapatupad ng security at privacy boundaries. Nangangahulugan ito na maaari mong patakbuhin ang iyong mga agents sa isang secure at kontroladong environment, na tinitiyak na maaari silang makipag-ugnayan nang ligtas at mahusay. Mayroong dalawang runtime na mahalaga:
  - **Stand-alone runtime**. Ito ay isang magandang pagpipilian para sa single-process applications kung saan lahat ng agents ay na-implement sa parehong programming language at tumatakbo sa parehong proseso. Narito ang isang ilustrasyon kung paano ito gumagana:

Application stack

*ang mga agents ay nagko-communicate sa pamamagitan ng mga mensahe sa runtime, at ang runtime ang nagma-manage ng lifecycle ng mga agents*

  - **Distributed agent runtime**, angkop para sa multi-process applications kung saan ang mga agents ay maaaring na-implement sa iba't ibang programming languages at tumatakbo sa iba't ibang makina. Narito ang isang ilustrasyon kung paano ito gumagana:

## Semantic Kernel + Agent Framework

Ang Semantic Kernel ay isang enterprise-ready AI Orchestration SDK. Binubuo ito ng AI at memory connectors, kasama ang isang Agent Framework.

Unahin nating talakayin ang ilang core components:

- **AI Connectors**: Ito ay isang interface sa mga external AI services at data sources para magamit sa parehong Python at C#.

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

    Narito ang isang simpleng halimbawa kung paano ka makakagawa ng kernel at magdagdag ng chat completion service. Ang Semantic Kernel ay lumilikha ng koneksyon sa isang external AI service, sa kasong ito, Azure OpenAI Chat Completion.

- **Plugins**: Ang mga ito ay nag-e-encapsulate ng mga function na maaaring gamitin ng isang application. Mayroong parehong ready-made plugins at custom na maaari mong likhain. Ang isang kaugnay na konsepto ay "prompt functions." Sa halip na magbigay ng natural language cues para sa function invocation, ibinobroadcast mo ang ilang mga function sa model. Batay sa kasalukuyang chat context, maaaring piliin ng model na tawagin ang isa sa mga function na ito upang kumpletuhin ang isang request o query. Narito ang isang halimbawa:

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

    Narito, mayroon kang isang template prompt na `skPrompt` na nagbibigay ng espasyo para sa user na mag-input ng text, `$userInput`. Pagkatapos ay nilikha mo ang kernel function na `SummarizeText` at pagkatapos ay in-import ito sa kernel gamit ang plugin name na `SemanticFunctions`. Tandaan ang pangalan ng function na tumutulong sa Semantic Kernel na maunawaan kung ano ang ginagawa ng function at kailan ito dapat tawagin.

- **Native function**: Mayroon ding native functions na maaaring tawagin ng framework nang direkta upang maisagawa ang gawain. Narito ang isang halimbawa ng ganitong function na kumukuha ng content mula sa isang file:

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

- **Memory**: Ina-abstract at pinapasimple ang context management para sa AI apps. Ang ideya sa memory ay ito ang dapat malaman ng LLM. Maaari mong i-store ang impormasyong ito sa isang vector store na nagiging isang in-memory database o isang vector database o katulad. Narito ang isang halimbawa ng isang napakasimpleng scenario kung saan ang *facts* ay idinadagdag sa memory:

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

    Ang mga facts na ito ay pagkatapos ay ini-store sa memory collection na `SummarizedAzureDocs`. Ito ay isang napakasimpleng halimbawa, ngunit makikita mo kung paano mo mai-store ang impormasyon sa memory para magamit ng LLM.
## Azure AI Agent Service

Ang Azure AI Agent Service ay isang mas bagong karagdagan, ipinakilala sa Microsoft Ignite 2024. Pinapayagan nito ang pagbuo at pag-deploy ng mga AI agent gamit ang mas flexible na mga modelo, tulad ng direktang pagtawag sa mga open-source LLMs tulad ng Llama 3, Mistral, at Cohere.

Ang Azure AI Agent Service ay nagbibigay ng mas malakas na mekanismo ng seguridad para sa enterprise at mga pamamaraan ng pag-iimbak ng data, na angkop para sa mga aplikasyon ng enterprise.

Ito ay gumagana agad-agad sa mga multi-agent orchestration frameworks tulad ng AutoGen at Semantic Kernel.

Ang serbisyong ito ay kasalukuyang nasa Public Preview at sumusuporta sa Python at C# para sa pagbuo ng mga agent.

Gamit ang Semantic Kernel Python, maaari tayong lumikha ng Azure AI Agent gamit ang isang user-defined plugin:

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

### Mga Pangunahing Konsepto

Ang Azure AI Agent Service ay may mga sumusunod na pangunahing konsepto:

- **Agent**. Ang Azure AI Agent Service ay isinama sa Azure AI Foundry. Sa loob ng AI Foundry, ang isang AI Agent ay kumikilos bilang isang "matalinong" microservice na maaaring gamitin upang sagutin ang mga tanong (RAG), magsagawa ng mga aksyon, o ganap na i-automate ang mga workflow. Nakakamit nito ito sa pamamagitan ng pagsasama ng kapangyarihan ng generative AI models sa mga tools na nagbibigay-daan dito na ma-access at makipag-ugnayan sa mga real-world data sources. Narito ang isang halimbawa ng agent:

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    Sa halimbawang ito, isang agent ang nilikha gamit ang modelong `gpt-4o-mini`, isang pangalan na `my-agent`, at mga tagubilin na `You are helpful agent`. Ang agent ay nilagyan ng mga tools at resources upang magsagawa ng mga code interpretation tasks.

- **Thread at mga mensahe**. Ang thread ay isa pang mahalagang konsepto. Ito ay kumakatawan sa isang pag-uusap o interaksyon sa pagitan ng isang agent at isang user. Ang mga thread ay maaaring gamitin upang subaybayan ang progreso ng pag-uusap, mag-imbak ng impormasyon ng konteksto, at pamahalaan ang estado ng interaksyon. Narito ang isang halimbawa ng thread:

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

    Sa nakaraang code, isang thread ang nilikha. Pagkatapos nito, isang mensahe ang ipinadala sa thread. Sa pamamagitan ng pagtawag sa `create_and_process_run`, ang agent ay hiniling na magsagawa ng trabaho sa thread. Sa huli, ang mga mensahe ay kinukuha at ina-log upang makita ang tugon ng agent. Ang mga mensahe ay nagpapahiwatig ng progreso ng pag-uusap sa pagitan ng user at ng agent. Mahalagang maunawaan na ang mga mensahe ay maaaring iba't ibang uri tulad ng text, image, o file, na ang resulta ng trabaho ng agent ay halimbawa isang imahe o text response. Bilang developer, maaari mong gamitin ang impormasyong ito upang higit pang iproseso ang tugon o ipakita ito sa user.

- **Pagsasama sa iba pang AI frameworks**. Ang Azure AI Agent Service ay maaaring makipag-ugnayan sa iba pang frameworks tulad ng AutoGen at Semantic Kernel, na nangangahulugang maaari kang bumuo ng bahagi ng iyong app sa isa sa mga frameworks na ito at halimbawa gamitin ang Agent Service bilang isang orchestrator o maaari mong buuin ang lahat sa Agent Service.

**Mga Gamit**: Ang Azure AI Agent Service ay idinisenyo para sa mga aplikasyon ng enterprise na nangangailangan ng secure, scalable, at flexible na AI agent deployment.

## Ano ang pagkakaiba ng mga frameworks na ito?

Mukhang may maraming pagkakapareho sa pagitan ng mga frameworks na ito, ngunit may ilang pangunahing pagkakaiba sa kanilang disenyo, kakayahan, at target na mga gamit:

- **AutoGen**: Isang experimentation framework na nakatuon sa cutting-edge na pananaliksik sa multi-agent systems. Ito ang pinakamahusay na lugar upang mag-eksperimento at mag-prototype ng mga sopistikadong multi-agent systems.
- **Semantic Kernel**: Isang production-ready agent library para sa pagbuo ng mga enterprise agentic applications. Nakatuon sa event-driven, distributed agentic applications, na nagbibigay-daan sa maraming LLMs at SLMs, tools, at single/multi-agent design patterns.
- **Azure AI Agent Service**: Isang platform at deployment service sa Azure Foundry para sa mga agent. Nag-aalok ng koneksyon sa mga serbisyo na sinusuportahan ng Azure tulad ng Azure OpenAI, Azure AI Search, Bing Search, at code execution.

Hindi pa rin sigurado kung alin ang pipiliin?

### Mga Gamit

Tingnan natin kung makakatulong kami sa pamamagitan ng pagdaan sa ilang karaniwang mga gamit:

> Q: Nag-eeksperimento ako, natututo, at bumubuo ng proof-of-concept agent applications, at gusto kong makabuo at mag-eksperimento nang mabilis
>

>A: Ang AutoGen ay magiging magandang pagpipilian para sa senaryong ito, dahil nakatuon ito sa event-driven, distributed agentic applications at sumusuporta sa advanced multi-agent design patterns.

> Q: Ano ang nagpapaganda sa AutoGen kumpara sa Semantic Kernel at Azure AI Agent Service para sa gamit na ito?
>
> A: Ang AutoGen ay partikular na idinisenyo para sa event-driven, distributed agentic applications, na angkop para sa pag-automate ng code generation at data analysis tasks. Nagbibigay ito ng mga kinakailangang tools at kakayahan upang mahusay na makabuo ng mga kumplikadong multi-agent systems.

>Q: Mukhang ang Azure AI Agent Service ay maaaring gumana rin dito, mayroon itong mga tools para sa code generation at iba pa?

>
> A: Oo, ang Azure AI Agent Service ay isang platform service para sa mga agent at may built-in na kakayahan para sa maraming modelo, Azure AI Search, Bing Search, at Azure Functions. Pinapadali nito ang pagbuo ng iyong mga agent sa Foundry Portal at ang pag-deploy sa kanila sa scale.

> Q: Nalilito pa rin ako, bigyan mo na lang ako ng isang opsyon
>
> A: Isang magandang pagpipilian ay buuin ang iyong aplikasyon sa Semantic Kernel muna at pagkatapos ay gamitin ang Azure AI Agent Service upang i-deploy ang iyong agent. Ang approach na ito ay nagbibigay-daan sa iyo na madaling i-persist ang iyong mga agent habang ginagamit ang kapangyarihan ng pagbuo ng multi-agent systems sa Semantic Kernel. Bukod pa rito, ang Semantic Kernel ay may connector sa AutoGen, na nagpapadali sa paggamit ng parehong frameworks nang magkasama.

I-summarize natin ang mga pangunahing pagkakaiba sa isang talahanayan:

| Framework | Pokus | Pangunahing Konsepto | Mga Gamit |
| --- | --- | --- | --- |
| AutoGen | Event-driven, distributed agentic applications | Agents, Personas, Functions, Data | Code generation, data analysis tasks |
| Semantic Kernel | Pag-unawa at pagbuo ng human-like na text content | Agents, Modular Components, Collaboration | Natural language understanding, content generation |
| Azure AI Agent Service | Flexible models, enterprise security, Code generation, Tool calling | Modularity, Collaboration, Process Orchestration | Secure, scalable, at flexible na AI agent deployment |

Ano ang ideal na gamit para sa bawat isa sa mga frameworks na ito?

## Maaari ko bang direktang isama ang aking mga kasalukuyang Azure ecosystem tools, o kailangan ko ng standalone solutions?

Ang sagot ay oo, maaari mong direktang isama ang iyong mga kasalukuyang Azure ecosystem tools sa Azure AI Agent Service lalo na, dahil ito ay itinayo upang gumana nang seamless sa iba pang Azure services. Halimbawa, maaari mong isama ang Bing, Azure AI Search, at Azure Functions. Mayroon ding malalim na integration sa Azure AI Foundry.

Para sa AutoGen at Semantic Kernel, maaari mo ring isama ang Azure services, ngunit maaaring kailanganin mong tawagan ang Azure services mula sa iyong code. Isa pang paraan ng pagsasama ay ang paggamit ng Azure SDKs upang makipag-ugnayan sa Azure services mula sa iyong mga agent. Bukod pa rito, tulad ng nabanggit, maaari mong gamitin ang Azure AI Agent Service bilang isang orchestrator para sa iyong mga agent na binuo sa AutoGen o Semantic Kernel na magbibigay ng madaling access sa Azure ecosystem.

### May Karagdagang Tanong Tungkol sa AI Agent Frameworks?

Sumali sa [Azure AI Foundry Discord](https://aka.ms/ai-agents/discord) upang makipagtagpo sa iba pang mga nag-aaral, dumalo sa office hours, at makuha ang mga sagot sa iyong mga tanong tungkol sa AI Agents.

## Mga Sanggunian

- ## Nakaraang Aralin

[Introduction to AI Agents and Agent Use Cases](../01-intro-to-ai-agents/README.md)

## Susunod na Aralin

[Understanding Agentic Design Patterns](../03-agentic-design-patterns/README.md)

---

**Paunawa**:  
Ang dokumentong ito ay isinalin gamit ang AI translation service na [Co-op Translator](https://github.com/Azure/co-op-translator). Bagama't sinisikap naming maging tumpak, pakitandaan na ang mga awtomatikong pagsasalin ay maaaring maglaman ng mga pagkakamali o hindi pagkakatugma. Ang orihinal na dokumento sa orihinal nitong wika ang dapat ituring na opisyal na sanggunian. Para sa mahalagang impormasyon, inirerekomenda ang propesyonal na pagsasalin ng tao. Hindi kami mananagot sa anumang hindi pagkakaunawaan o maling interpretasyon na maaaring magmula sa paggamit ng pagsasaling ito.