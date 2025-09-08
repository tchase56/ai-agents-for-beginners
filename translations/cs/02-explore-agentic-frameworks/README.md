<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-29T20:27:35+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "cs"
}
-->
[![Zkoumání rámců AI agentů](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.cs.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(Klikněte na obrázek výše pro zhlédnutí videa této lekce)_

# Prozkoumejte rámce AI agentů

Rámce AI agentů jsou softwarové platformy navržené tak, aby usnadnily tvorbu, nasazení a správu AI agentů. Tyto rámce poskytují vývojářům předem připravené komponenty, abstrakce a nástroje, které zjednodušují vývoj složitých AI systémů.

Tyto rámce pomáhají vývojářům soustředit se na jedinečné aspekty jejich aplikací tím, že nabízejí standardizované přístupy k běžným výzvám při vývoji AI agentů. Zvyšují škálovatelnost, přístupnost a efektivitu při budování AI systémů.

## Úvod

Tato lekce pokryje:

- Co jsou rámce AI agentů a co umožňují vývojářům dosáhnout?
- Jak mohou týmy tyto rámce využít k rychlému prototypování, iteraci a zlepšování schopností jejich agentů?
- Jaké jsou rozdíly mezi rámci a nástroji vytvořenými společností Microsoft, a dalšími?
- Mohu integrovat své stávající nástroje Azure přímo, nebo potřebuji samostatná řešení?
- Co je služba Azure AI Agents a jak mi pomáhá?

## Cíle učení

Cíle této lekce jsou pomoci vám pochopit:

- Roli rámců AI agentů ve vývoji AI.
- Jak využít rámce AI agentů k budování inteligentních agentů.
- Klíčové schopnosti umožněné rámci AI agentů.
- Rozdíly mezi AutoGen, Semantic Kernel a Azure AI Agent Service.

## Co jsou rámce AI agentů a co umožňují vývojářům dělat?

Tradiční AI rámce vám mohou pomoci integrovat AI do vašich aplikací a zlepšit je následujícími způsoby:

- **Personalizace**: AI může analyzovat chování a preference uživatelů a poskytovat personalizovaná doporučení, obsah a zážitky.  
Příklad: Streamovací služby jako Netflix používají AI k doporučování filmů a seriálů na základě historie sledování, čímž zvyšují zapojení a spokojenost uživatelů.
- **Automatizace a efektivita**: AI může automatizovat opakující se úkoly, zjednodušovat pracovní postupy a zlepšovat provozní efektivitu.  
Příklad: Aplikace zákaznické podpory využívají chatboty poháněné AI k řešení běžných dotazů, čímž zkracují dobu odezvy a uvolňují lidské agenty pro složitější problémy.
- **Vylepšený uživatelský zážitek**: AI může zlepšit celkový uživatelský zážitek poskytováním inteligentních funkcí, jako je rozpoznávání hlasu, zpracování přirozeného jazyka a prediktivní text.  
Příklad: Virtuální asistenti jako Siri a Google Assistant využívají AI k porozumění a reakci na hlasové příkazy, což uživatelům usnadňuje interakci s jejich zařízeními.

### To všechno zní skvěle, tak proč potřebujeme rámce AI agentů?

Rámce AI agentů představují něco víc než jen AI rámce. Jsou navrženy tak, aby umožnily tvorbu inteligentních agentů, kteří mohou interagovat s uživateli, jinými agenty a prostředím za účelem dosažení konkrétních cílů. Tito agenti mohou vykazovat autonomní chování, činit rozhodnutí a přizpůsobovat se měnícím se podmínkám. Podívejme se na některé klíčové schopnosti umožněné rámci AI agentů:

- **Spolupráce a koordinace agentů**: Umožňuje tvorbu více AI agentů, kteří mohou spolupracovat, komunikovat a koordinovat se při řešení složitých úkolů.
- **Automatizace a správa úkolů**: Poskytuje mechanismy pro automatizaci vícestupňových pracovních postupů, delegování úkolů a dynamickou správu úkolů mezi agenty.
- **Porozumění kontextu a adaptace**: Vybavuje agenty schopností porozumět kontextu, přizpůsobit se měnícímu se prostředí a činit rozhodnutí na základě informací v reálném čase.

Shrnuto, agenti vám umožňují dělat více, posunout automatizaci na další úroveň a vytvářet inteligentnější systémy, které se mohou učit a přizpůsobovat svému prostředí.

## Jak rychle prototypovat, iterovat a zlepšovat schopnosti agentů?

Toto je rychle se vyvíjející oblast, ale existují některé společné prvky napříč většinou rámců AI agentů, které vám mohou pomoci rychle prototypovat a iterovat, konkrétně modulární komponenty, kolaborativní nástroje a učení v reálném čase. Pojďme se na ně podívat:

- **Používejte modulární komponenty**: AI SDK nabízejí předem připravené komponenty, jako jsou AI a paměťové konektory, volání funkcí pomocí přirozeného jazyka nebo pluginů kódu, šablony promptů a další.
- **Využívejte kolaborativní nástroje**: Navrhujte agenty s konkrétními rolemi a úkoly, což umožňuje testování a zdokonalování kolaborativních pracovních postupů.
- **Učte se v reálném čase**: Implementujte zpětnovazební smyčky, kde se agenti učí z interakcí a dynamicky přizpůsobují své chování.

### Používejte modulární komponenty

SDK jako Microsoft Semantic Kernel a LangChain nabízejí předem připravené komponenty, jako jsou AI konektory, šablony promptů a správa paměti.

**Jak to mohou týmy využít**: Týmy mohou rychle sestavit tyto komponenty a vytvořit funkční prototyp bez nutnosti začínat od nuly, což umožňuje rychlé experimentování a iteraci.

**Jak to funguje v praxi**: Můžete použít předem připravený parser k extrakci informací ze vstupu uživatele, paměťový modul k ukládání a načítání dat a generátor promptů k interakci s uživateli, aniž byste museli tyto komponenty vytvářet od nuly.

**Příklad kódu**. Podívejme se na příklady, jak můžete použít předem připravený AI konektor se Semantic Kernel Python a .Net, který využívá automatické volání funkcí, aby model reagoval na vstup uživatele:

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

Z tohoto příkladu vidíte, jak můžete využít předem připravený parser k extrakci klíčových informací ze vstupu uživatele, jako je původ, cíl a datum požadavku na rezervaci letu. Tento modulární přístup vám umožňuje soustředit se na logiku na vyšší úrovni.

### Využívejte kolaborativní nástroje

Rámce jako CrewAI, Microsoft AutoGen a Semantic Kernel usnadňují tvorbu více agentů, kteří mohou spolupracovat.

**Jak to mohou týmy využít**: Týmy mohou navrhovat agenty s konkrétními rolemi a úkoly, což umožňuje testování a zdokonalování kolaborativních pracovních postupů a zlepšení celkové efektivity systému.

**Jak to funguje v praxi**: Můžete vytvořit tým agentů, kde každý agent má specializovanou funkci, jako je získávání dat, analýza nebo rozhodování. Tito agenti mohou komunikovat a sdílet informace za účelem dosažení společného cíle, jako je zodpovězení dotazu uživatele nebo dokončení úkolu.

**Příklad kódu (AutoGen)**:

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

V předchozím kódu vidíte, jak můžete vytvořit úkol, který zahrnuje více agentů spolupracujících na analýze dat. Každý agent vykonává specifickou funkci a úkol je proveden koordinací agentů za účelem dosažení požadovaného výsledku. Vytvořením specializovaných agentů můžete zlepšit efektivitu a výkon úkolů.

### Učte se v reálném čase

Pokročilé rámce poskytují schopnosti pro porozumění kontextu a adaptaci v reálném čase.

**Jak to mohou týmy využít**: Týmy mohou implementovat zpětnovazební smyčky, kde se agenti učí z interakcí a dynamicky přizpůsobují své chování, což vede k neustálému zlepšování a zdokonalování schopností.

**Jak to funguje v praxi**: Agenti mohou analyzovat zpětnou vazbu uživatelů, data z prostředí a výsledky úkolů, aby aktualizovali svou znalostní bázi, přizpůsobili algoritmy rozhodování a zlepšili výkon v průběhu času. Tento iterativní proces učení umožňuje agentům přizpůsobit se měnícím se podmínkám a preferencím uživatelů, čímž se zvyšuje celková efektivita systému.

## Jaké jsou rozdíly mezi rámci AutoGen, Semantic Kernel a Azure AI Agent Service?

Existuje mnoho způsobů, jak tyto rámce porovnat, ale podívejme se na některé klíčové rozdíly z hlediska jejich návrhu, schopností a cílových případů použití:

## AutoGen

AutoGen je open-source rámec vyvinutý laboratoří Microsoft Research's AI Frontiers Lab. Zaměřuje se na událostmi řízené, distribuované *agentní* aplikace, umožňující více LLMs a SLMs, nástroje a pokročilé návrhové vzory pro více agentů.

AutoGen je postaven kolem základního konceptu agentů, což jsou autonomní entity, které mohou vnímat své prostředí, činit rozhodnutí a podnikat kroky k dosažení konkrétních cílů. Agenti komunikují prostřednictvím asynchronních zpráv, což jim umožňuje pracovat nezávisle a paralelně, čímž se zvyšuje škálovatelnost a odezva systému.

Podle Wikipedie je herec _základním stavebním kamenem souběžného výpočtu. V reakci na přijatou zprávu může herec: činit lokální rozhodnutí, vytvářet další herce, posílat další zprávy a určovat, jak reagovat na další přijatou zprávu_.

**Případy použití**: Automatizace generování kódu, úkoly analýzy dat a tvorba vlastních agentů pro plánování a výzkumné funkce.

Zde jsou některé důležité základní koncepty AutoGen:

- **Agenti**. Agent je softwarová entita, která:  
  - **Komunikuje prostřednictvím zpráv**, které mohou být synchronní nebo asynchronní.  
  - **Udržuje svůj vlastní stav**, který může být upraven příchozími zprávami.  
  - **Provádí akce** v reakci na přijaté zprávy nebo změny svého stavu. Tyto akce mohou upravit stav agenta a vyvolat externí efekty, jako je aktualizace záznamů zpráv, odesílání nových zpráv, spouštění kódu nebo volání API.

  Zde je krátký úryvek kódu, ve kterém vytvoříte svého vlastního agenta s chatovacími schopnostmi:

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

    V předchozím kódu byl vytvořen `MyAssistant`, který dědí z `RoutedAgent`. Má obslužnou rutinu zpráv, která tiskne obsah zprávy a poté odešle odpověď pomocí delegáta `AssistantAgent`. Zvláště si všimněte, jak přiřazujeme `self._delegate` instanci `AssistantAgent`, což je předem připravený agent, který zvládá dokončování chatu.

    Pojďme nyní informovat AutoGen o tomto typu agenta a spustit program:

    ```python
    
    # main.py
    runtime = SingleThreadedAgentRuntime()
    await MyAgent.register(runtime, "my_agent", lambda: MyAgent())

    runtime.start()  # Start processing messages in the background.
    await runtime.send_message(MyMessageType("Hello, World!"), AgentId("my_agent", "default"))
    ```

    V předchozím kódu jsou agenti zaregistrováni v runtime a poté je agentovi odeslána zpráva, což vede k následujícímu výstupu:

    ```text
    # Output from the console:
    my_agent received message: Hello, World!
    my_assistant received message: Hello, World!
    my_assistant responded: Hello! How can I assist you today?
    ```

- **Více agentů**. AutoGen podporuje tvorbu více agentů, kteří mohou spolupracovat na dosažení složitých úkolů. Agenti mohou komunikovat, sdílet informace a koordinovat své akce, aby efektivněji řešili problémy. Pro vytvoření systému s více agenty můžete definovat různé typy agentů se specializovanými funkcemi a rolemi, jako je získávání dat, analýza, rozhodování a interakce s uživatelem. Podívejme se, jak taková tvorba vypadá:

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

    V předchozím kódu máme `GroupChatManager`, který je zaregistrován v runtime. Tento manažer je zodpovědný za koordinaci interakcí mezi různými typy agentů, jako jsou spisovatelé, ilustrátoři, editoři a uživatelé.

- **Agentní runtime**. Rámec poskytuje runtime prostředí, které umožňuje komunikaci mezi agenty, spravuje jejich identity a životní cykly a zajišťuje bezpečnostní a soukromé hranice. To znamená, že můžete spouštět své agenty v bezpečném a kontrolovaném prostředí, což zajišťuje, že mohou bezpečně a efektivně interagovat. Existují dva zajímavé runtime:
  - **Samostatný runtime**. Toto je dobrá volba pro aplikace s jedním procesem, kde jsou všichni agenti implementováni ve stejném programovacím jazyce a běží ve stejném procesu. Zde je ilustrace, jak to funguje:

    Aplikační stack

    *agenti komunikují prostřednictvím zpráv přes runtime, který spravuje životní cyklus agentů*

  - **Distribuovaný agentní runtime**, je vhodný pro aplikace s více procesy, kde mohou být agenti implementováni v různých programovacích jazycích a běžet na různých strojích. Zde je ilustrace, jak to funguje:

## Semantic Kernel + Agent Framework

Semantic Kernel je podnikový AI Orchestration SDK. Skládá se z AI a paměťových konektorů spolu s Agent Frameworkem.

Nejprve si pokryjme některé základní komponenty:

- **AI konektory**: Toto je rozhraní s externími AI službami a datovými zdroji pro použití v Pythonu i C#.

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

    Zde máte jednoduchý příklad, jak můžete vytvořit kernel a přidat službu dokončování chatu. Semantic Kernel vytváří připojení k externí AI službě, v tomto případě Azure OpenAI Chat Completion.

- **Pluginy**: Tyto zapouzdřují funkce, které může aplikace používat. Existují jak hotové pluginy, tak vlastní, které si můžete vytvořit. Souvisejícím konceptem jsou "prompt functions". Místo poskytování přirozených jazykových podnětů pro vyvolání funkcí vysíláte určité funkce modelu. Na základě aktuálního kontextu chatu může model zvolit volání jedné z těchto funkcí k dokončení požadavku nebo dotazu. Zde je příklad:

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

    Zde nejprve máte šablonu promptu `skPrompt`, která ponechává prostor pro vstup uživatele, `$userInput`. Poté vytvoříte kernel funkci `SummarizeText` a importujete ji do kernelu s názvem pluginu `SemanticFunctions`. Všimněte si názvu funkce, který pomáhá Semantic Kernel pochopit, co funkce dělá a kdy by měla být volána.

- **Nativní funkce**: Existují také nativní funkce, které může rámec přímo volat k provedení úkolu. Zde je příklad takové funkce, která načítá obsah ze souboru:

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

- **Paměť**: Abstrahuje a zjednodušuje správu kontextu pro AI aplikace. Myšlenka paměti je, že jde o něco, co by LLM mělo vědět. Tyto informace můžete uložit do vektorového úložiště, což je buď databáze v paměti, nebo vektorová databáze či podobné. Zde je příklad velmi zjednodušeného scénáře, kde jsou *fakta* přidána do paměti:

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

    Tato fakta jsou pot
Tak to jsou základy rámce Semantic Kernel, co ale Agent Framework?

## Azure AI Agent Service

Azure AI Agent Service je novější přírůstek, představený na Microsoft Ignite 2024. Umožňuje vývoj a nasazení AI agentů s flexibilnějšími modely, například přímým voláním open-source LLM jako Llama 3, Mistral a Cohere.

Azure AI Agent Service poskytuje silnější mechanismy zabezpečení pro podniky a metody ukládání dat, což ho činí vhodným pro podnikové aplikace.

Funguje ihned po instalaci s orchestračními rámci pro více agentů, jako jsou AutoGen a Semantic Kernel.

Tato služba je momentálně ve veřejném náhledu a podporuje Python a C# pro tvorbu agentů.

Pomocí Semantic Kernel Python můžeme vytvořit Azure AI Agent s uživatelsky definovaným pluginem:

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

### Základní koncepty

Azure AI Agent Service má následující základní koncepty:

- **Agent**. Azure AI Agent Service se integruje s Azure AI Foundry. V rámci AI Foundry funguje AI Agent jako „chytrá“ mikroslužba, kterou lze použít k odpovídání na otázky (RAG), provádění akcí nebo úplné automatizaci pracovních postupů. Toho dosahuje kombinací síly generativních AI modelů s nástroji, které mu umožňují přístup k reálným datovým zdrojům a interakci s nimi. Zde je příklad agenta:

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    V tomto příkladu je agent vytvořen s modelem `gpt-4o-mini`, názvem `my-agent` a instrukcemi `You are helpful agent`. Agent je vybaven nástroji a zdroji pro provádění úkolů interpretace kódu.

- **Vlákno a zprávy**. Vlákno je dalším důležitým konceptem. Představuje konverzaci nebo interakci mezi agentem a uživatelem. Vlákna lze použít ke sledování průběhu konverzace, ukládání kontextových informací a správě stavu interakce. Zde je příklad vlákna:

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

    V předchozím kódu je vytvořeno vlákno. Poté je do vlákna odeslána zpráva. Voláním `create_and_process_run` je agent požádán, aby provedl práci na vlákně. Nakonec jsou zprávy získány a zaznamenány, aby bylo vidět odpověď agenta. Zprávy ukazují průběh konverzace mezi uživatelem a agentem. Je také důležité pochopit, že zprávy mohou mít různé typy, jako je text, obrázek nebo soubor, což znamená, že práce agenta vedla například k vytvoření obrázku nebo textové odpovědi. Jako vývojář můžete tyto informace dále zpracovat nebo je prezentovat uživateli.

- **Integrace s jinými AI rámci**. Azure AI Agent Service může interagovat s jinými rámci, jako jsou AutoGen a Semantic Kernel, což znamená, že můžete část své aplikace vytvořit v jednom z těchto rámců a například použít Agent Service jako orchestrátor, nebo můžete vše vytvořit v Agent Service.

**Použití**: Azure AI Agent Service je navržen pro podnikové aplikace, které vyžadují bezpečné, škálovatelné a flexibilní nasazení AI agentů.

## Jaký je rozdíl mezi těmito rámci?

Zdá se, že mezi těmito rámci existuje mnoho překryvů, ale existují klíčové rozdíly v jejich designu, schopnostech a cílových případech použití:

- **AutoGen**: Je experimentální rámec zaměřený na špičkový výzkum systémů s více agenty. Je to nejlepší místo pro experimentování a prototypování sofistikovaných systémů s více agenty.
- **Semantic Kernel**: Je produkčně připravená knihovna agentů pro tvorbu podnikových agentních aplikací. Zaměřuje se na událostmi řízené, distribuované agentní aplikace, umožňuje použití více LLM a SLM, nástrojů a návrhových vzorů pro jednoho nebo více agentů.
- **Azure AI Agent Service**: Je platforma a služba pro nasazení agentů v Azure Foundry. Nabízí budování konektivity ke službám podporovaným Azure, jako jsou Azure OpenAI, Azure AI Search, Bing Search a provádění kódu.

Stále si nejste jisti, který zvolit?

### Použití

Podívejme se, jestli vám můžeme pomoci projít některé běžné případy použití:

> Q: Experimentuji, učím se a vytvářím proof-of-concept aplikace agentů a chci být schopen rychle stavět a experimentovat
>

>A: AutoGen by byl dobrá volba pro tento scénář, protože se zaměřuje na událostmi řízené, distribuované agentní aplikace a podporuje pokročilé návrhové vzory pro více agentů.

> Q: Co dělá AutoGen lepší volbou než Semantic Kernel a Azure AI Agent Service pro tento případ použití?
>
> A: AutoGen je speciálně navržen pro událostmi řízené, distribuované agentní aplikace, což ho činí dobře vhodným pro automatizaci úkolů generování kódu a analýzy dat. Poskytuje potřebné nástroje a schopnosti pro efektivní tvorbu komplexních systémů s více agenty.

>Q: Zní to, že Azure AI Agent Service by zde také mohl fungovat, má nástroje pro generování kódu a další?
>
> A: Ano, Azure AI Agent Service je platformová služba pro agenty a přidává vestavěné schopnosti pro více modelů, Azure AI Search, Bing Search a Azure Functions. Umožňuje snadno vytvářet vaše agenty v Foundry Portálu a nasazovat je ve velkém měřítku.

> Q: Pořád jsem zmatený, dejte mi jen jednu možnost
>
> A: Skvělou volbou je nejprve vytvořit vaši aplikaci v Semantic Kernel a poté použít Azure AI Agent Service k nasazení vašeho agenta. Tento přístup vám umožní snadno uchovávat vaše agenty a zároveň využívat sílu k vytvoření systémů s více agenty v Semantic Kernel. Navíc má Semantic Kernel konektor v AutoGen, což usnadňuje použití obou rámců společně.

Shrňme klíčové rozdíly v tabulce:

| Rámec | Zaměření | Základní koncepty | Případy použití |
| --- | --- | --- | --- |
| AutoGen | Událostmi řízené, distribuované agentní aplikace | Agenti, Persony, Funkce, Data | Generování kódu, úkoly analýzy dat |
| Semantic Kernel | Porozumění a generování textového obsahu podobného lidskému | Agenti, Modulární komponenty, Spolupráce | Porozumění přirozenému jazyku, generování obsahu |
| Azure AI Agent Service | Flexibilní modely, podniková bezpečnost, Generování kódu, Volání nástrojů | Modularita, Spolupráce, Orchestrace procesů | Bezpečné, škálovatelné a flexibilní nasazení AI agentů |

Jaký je ideální případ použití pro každý z těchto rámců?

## Mohu integrovat své stávající nástroje Azure ekosystému přímo, nebo potřebuji samostatná řešení?

Odpověď je ano, můžete integrovat své stávající nástroje Azure ekosystému přímo s Azure AI Agent Service, zejména proto, že byl vytvořen tak, aby bezproblémově fungoval s ostatními službami Azure. Můžete například integrovat Bing, Azure AI Search a Azure Functions. Existuje také hluboká integrace s Azure AI Foundry.

Pro AutoGen a Semantic Kernel můžete také integrovat s Azure službami, ale může být nutné volat Azure služby z vašeho kódu. Dalším způsobem integrace je použití Azure SDKs k interakci s Azure službami z vašich agentů. Navíc, jak bylo zmíněno, můžete použít Azure AI Agent Service jako orchestrátor pro vaše agenty vytvořené v AutoGen nebo Semantic Kernel, což by poskytlo snadný přístup k Azure ekosystému.

### Máte další otázky ohledně AI Agent Frameworks?

Připojte se k [Azure AI Foundry Discord](https://aka.ms/ai-agents/discord), kde se můžete setkat s ostatními studenty, zúčastnit se konzultačních hodin a získat odpovědi na vaše otázky ohledně AI agentů.

## Reference

- 

## Předchozí lekce

[Úvod do AI agentů a jejich případů použití](../01-intro-to-ai-agents/README.md)

## Další lekce

[Porozumění návrhovým vzorům agentů](../03-agentic-design-patterns/README.md)

---

**Prohlášení**:  
Tento dokument byl přeložen pomocí služby pro automatický překlad [Co-op Translator](https://github.com/Azure/co-op-translator). I když se snažíme o co největší přesnost, mějte prosím na paměti, že automatické překlady mohou obsahovat chyby nebo nepřesnosti. Původní dokument v jeho původním jazyce by měl být považován za závazný zdroj. Pro důležité informace doporučujeme profesionální lidský překlad. Neodpovídáme za žádná nedorozumění nebo nesprávné výklady vyplývající z použití tohoto překladu.