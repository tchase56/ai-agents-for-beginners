<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-29T20:41:41+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "sk"
}
-->
[![Preskúmanie rámcov pre AI agentov](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.sk.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(Kliknite na obrázok vyššie pre zobrazenie videa k tejto lekcii)_

# Preskúmajte rámce pre AI agentov

Rámce pre AI agentov sú softvérové platformy navrhnuté na zjednodušenie tvorby, nasadenia a správy AI agentov. Tieto rámce poskytujú vývojárom predpripravené komponenty, abstrakcie a nástroje, ktoré uľahčujú vývoj komplexných AI systémov.

Tieto rámce pomáhajú vývojárom sústrediť sa na jedinečné aspekty ich aplikácií tým, že poskytujú štandardizované prístupy k bežným výzvam vo vývoji AI agentov. Zlepšujú škálovateľnosť, prístupnosť a efektivitu pri budovaní AI systémov.

## Úvod

Táto lekcia pokryje:

- Čo sú rámce pre AI agentov a čo umožňujú vývojárom dosiahnuť?
- Ako môžu tímy tieto rámce využiť na rýchle prototypovanie, iteráciu a zlepšovanie schopností svojich agentov?
- Aké sú rozdiely medzi rámcami a nástrojmi vytvorenými spoločnosťou Microsoft, Google a ďalšími?
- Môžem integrovať svoje existujúce nástroje ekosystému Azure priamo, alebo potrebujem samostatné riešenia?
- Čo je služba Azure AI Agents a ako mi pomáha?

## Ciele učenia

Ciele tejto lekcie sú pomôcť vám pochopiť:

- Úlohu rámcov pre AI agentov vo vývoji AI.
- Ako využiť rámce pre AI agentov na budovanie inteligentných agentov.
- Kľúčové schopnosti umožnené rámcami pre AI agentov.
- Rozdiely medzi AutoGen, Semantic Kernel a Azure AI Agent Service.

## Čo sú rámce pre AI agentov a čo umožňujú vývojárom robiť?

Tradičné AI rámce vám môžu pomôcť integrovať AI do vašich aplikácií a zlepšiť ich v nasledujúcich oblastiach:

- **Personalizácia**: AI dokáže analyzovať správanie a preferencie používateľov a poskytovať personalizované odporúčania, obsah a zážitky.  
Príklad: Streamovacie služby ako Netflix používajú AI na odporúčanie filmov a seriálov na základe histórie sledovania, čím zvyšujú angažovanosť a spokojnosť používateľov.
- **Automatizácia a efektivita**: AI dokáže automatizovať opakujúce sa úlohy, zjednodušiť pracovné postupy a zlepšiť operačnú efektivitu.  
Príklad: Aplikácie zákazníckeho servisu využívajú chatboty poháňané AI na riešenie bežných otázok, čím skracujú časy odozvy a uvoľňujú ľudských agentov na zložitejšie problémy.
- **Zlepšenie používateľského zážitku**: AI dokáže zlepšiť celkový používateľský zážitok poskytovaním inteligentných funkcií, ako je rozpoznávanie hlasu, spracovanie prirodzeného jazyka a prediktívny text.  
Príklad: Virtuálni asistenti ako Siri a Google Assistant využívajú AI na pochopenie a odpovedanie na hlasové príkazy, čím uľahčujú používateľom interakciu so zariadeniami.

### To všetko znie skvele, tak prečo potrebujeme rámce pre AI agentov?

Rámce pre AI agentov predstavujú niečo viac než len AI rámce. Sú navrhnuté tak, aby umožnili tvorbu inteligentných agentov, ktorí dokážu interagovať s používateľmi, inými agentmi a prostredím na dosiahnutie konkrétnych cieľov. Títo agenti môžu vykazovať autonómne správanie, robiť rozhodnutia a prispôsobovať sa meniacim sa podmienkam. Pozrime sa na niektoré kľúčové schopnosti umožnené rámcami pre AI agentov:

- **Spolupráca a koordinácia agentov**: Umožňujú tvorbu viacerých AI agentov, ktorí dokážu spolupracovať, komunikovať a koordinovať sa na riešení komplexných úloh.
- **Automatizácia a správa úloh**: Poskytujú mechanizmy na automatizáciu viacstupňových pracovných postupov, delegovanie úloh a dynamickú správu úloh medzi agentmi.
- **Kontextové porozumenie a adaptácia**: Vybavujú agentov schopnosťou porozumieť kontextu, prispôsobiť sa meniacemu sa prostrediu a robiť rozhodnutia na základe informácií v reálnom čase.

V skratke, agenti vám umožňujú robiť viac, posunúť automatizáciu na vyššiu úroveň a vytvárať inteligentnejšie systémy, ktoré sa dokážu učiť a prispôsobovať svojmu prostrediu.

## Ako rýchlo prototypovať, iterovať a zlepšovať schopnosti agenta?

Toto je rýchlo sa meniaca oblasť, ale existujú niektoré spoločné prvky naprieč väčšinou rámcov pre AI agentov, ktoré vám môžu pomôcť rýchlo prototypovať a iterovať, konkrétne modulárne komponenty, kolaboratívne nástroje a učenie v reálnom čase. Poďme sa na ne pozrieť:

- **Používajte modulárne komponenty**: AI SDK ponúkajú predpripravené komponenty, ako sú AI a pamäťové konektory, volanie funkcií pomocou prirodzeného jazyka alebo kódových pluginov, šablóny výziev a ďalšie.
- **Využívajte kolaboratívne nástroje**: Navrhujte agentov so špecifickými úlohami a rolami, čo umožňuje testovanie a zdokonaľovanie kolaboratívnych pracovných postupov.
- **Učte sa v reálnom čase**: Implementujte spätnoväzbové slučky, kde sa agenti učia z interakcií a dynamicky prispôsobujú svoje správanie.

### Používajte modulárne komponenty

SDK ako Microsoft Semantic Kernel a LangChain ponúkajú predpripravené komponenty, ako sú AI konektory, šablóny výziev a správa pamäte.

**Ako to môžu tímy využiť**: Tímy môžu rýchlo zostaviť tieto komponenty na vytvorenie funkčného prototypu bez potreby začínať od nuly, čo umožňuje rýchle experimentovanie a iteráciu.

**Ako to funguje v praxi**: Môžete použiť predpripravený parser na extrakciu informácií z používateľského vstupu, pamäťový modul na ukladanie a získavanie údajov a generátor výziev na interakciu s používateľmi, a to všetko bez potreby vytvárať tieto komponenty od nuly.

**Príklad kódu**. Pozrime sa na príklady, ako môžete použiť predpripravený AI konektor so Semantic Kernel Python a .Net, ktorý využíva automatické volanie funkcií na to, aby model reagoval na používateľský vstup:

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

Z tohto príkladu vidíte, ako môžete využiť predpripravený parser na extrakciu kľúčových informácií z používateľského vstupu, ako je pôvod, cieľ a dátum požiadavky na rezerváciu letu. Tento modulárny prístup vám umožňuje sústrediť sa na vyššiu logiku.

### Využívajte kolaboratívne nástroje

Rámce ako CrewAI, Microsoft AutoGen a Semantic Kernel uľahčujú tvorbu viacerých agentov, ktorí dokážu spolupracovať.

**Ako to môžu tímy využiť**: Tímy môžu navrhovať agentov so špecifickými úlohami a rolami, čo umožňuje testovanie a zdokonaľovanie kolaboratívnych pracovných postupov a zlepšenie celkovej efektivity systému.

**Ako to funguje v praxi**: Môžete vytvoriť tím agentov, kde každý agent má špecializovanú funkciu, ako je získavanie údajov, analýza alebo rozhodovanie. Títo agenti môžu komunikovať a zdieľať informácie na dosiahnutie spoločného cieľa, ako je odpovedanie na používateľskú otázku alebo dokončenie úlohy.

**Príklad kódu (AutoGen)**:

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

V predchádzajúcom kóde vidíte, ako môžete vytvoriť úlohu, ktorá zahŕňa viacerých agentov spolupracujúcich na analýze údajov. Každý agent vykonáva špecifickú funkciu a úloha sa vykonáva koordináciou agentov na dosiahnutie požadovaného výsledku. Vytváraním špecializovaných agentov môžete zlepšiť efektivitu a výkon úloh.

### Učte sa v reálnom čase

Pokročilé rámce poskytujú schopnosti na pochopenie kontextu a adaptáciu v reálnom čase.

**Ako to môžu tímy využiť**: Tímy môžu implementovať spätnoväzbové slučky, kde sa agenti učia z interakcií a dynamicky prispôsobujú svoje správanie, čo vedie k neustálemu zlepšovaniu a zdokonaľovaniu schopností.

**Ako to funguje v praxi**: Agenti môžu analyzovať spätnú väzbu používateľov, údaje z prostredia a výsledky úloh na aktualizáciu svojej databázy znalostí, prispôsobenie rozhodovacích algoritmov a zlepšenie výkonu v priebehu času. Tento iteratívny proces učenia umožňuje agentom prispôsobiť sa meniacim sa podmienkam a preferenciám používateľov, čím zvyšuje celkovú efektivitu systému.

## Aké sú rozdiely medzi rámcami AutoGen, Semantic Kernel a Azure AI Agent Service?

Existuje mnoho spôsobov, ako porovnať tieto rámce, ale pozrime sa na niektoré kľúčové rozdiely z hľadiska ich dizajnu, schopností a cieľových prípadov použitia:

## AutoGen

AutoGen je open-source rámec vyvinutý laboratóriom Microsoft Research's AI Frontiers Lab. Zameriava sa na udalostne riadené, distribuované *agentické* aplikácie, umožňujúce viacnásobné LLM a SLM, nástroje a pokročilé vzory dizajnu pre viac agentov.

AutoGen je postavený na základnom koncepte agentov, ktorí sú autonómnymi entitami schopnými vnímať svoje prostredie, robiť rozhodnutia a vykonávať akcie na dosiahnutie konkrétnych cieľov. Agenti komunikujú prostredníctvom asynchrónnych správ, čo im umožňuje pracovať nezávisle a paralelne, čím zvyšujú škálovateľnosť a odozvu systému.
Takže to sú základy rámca Semantic Kernel, čo však Agent Framework?

## Azure AI Agent Service

Azure AI Agent Service je novší prírastok, predstavený na Microsoft Ignite 2024. Umožňuje vývoj a nasadenie AI agentov s flexibilnejšími modelmi, ako je priame volanie open-source LLMs ako Llama 3, Mistral a Cohere.

Azure AI Agent Service poskytuje silnejšie mechanizmy podnikovej bezpečnosti a metódy ukladania dát, čo ho robí vhodným pre podnikové aplikácie.

Funguje okamžite s rámcami na orchestráciu multi-agentov, ako sú AutoGen a Semantic Kernel.

Táto služba je momentálne vo verejnom náhľade a podporuje Python a C# na tvorbu agentov.

Pomocou Semantic Kernel Python môžeme vytvoriť Azure AI Agent s pluginom definovaným používateľom:

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

### Základné koncepty

Azure AI Agent Service má nasledujúce základné koncepty:

- **Agent**. Azure AI Agent Service integruje s Azure AI Foundry. V rámci AI Foundry funguje AI Agent ako "inteligentná" mikroslužba, ktorú je možné použiť na odpovedanie na otázky (RAG), vykonávanie akcií alebo úplnú automatizáciu pracovných postupov. Dosahuje to kombináciou generatívnych AI modelov s nástrojmi, ktoré mu umožňujú prístup k reálnym dátovým zdrojom a interakciu s nimi. Tu je príklad agenta:

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    V tomto príklade je agent vytvorený s modelom `gpt-4o-mini`, názvom `my-agent` a inštrukciami `You are helpful agent`. Agent je vybavený nástrojmi a zdrojmi na vykonávanie úloh interpretácie kódu.

- **Vlákno a správy**. Vlákno je ďalší dôležitý koncept. Predstavuje konverzáciu alebo interakciu medzi agentom a používateľom. Vlákna môžu byť použité na sledovanie priebehu konverzácie, ukladanie kontextových informácií a správu stavu interakcie. Tu je príklad vlákna:

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

    V predchádzajúcom kóde je vytvorené vlákno. Následne je do vlákna odoslaná správa. Volaním `create_and_process_run` je agent požiadaný, aby vykonal prácu na vlákne. Nakoniec sú správy získané a zaznamenané, aby sa videla odpoveď agenta. Správy indikujú priebeh konverzácie medzi používateľom a agentom. Je tiež dôležité pochopiť, že správy môžu mať rôzne typy, ako text, obrázok alebo súbor, čo znamená, že práca agenta mohla viesť napríklad k obrázku alebo textovej odpovedi. Ako vývojár môžete tieto informácie ďalej spracovať alebo ich prezentovať používateľovi.

- **Integrácia s inými AI rámcami**. Azure AI Agent Service môže interagovať s inými rámcami, ako sú AutoGen a Semantic Kernel, čo znamená, že časť svojej aplikácie môžete vytvoriť v jednom z týchto rámcov a napríklad použiť Agent Service ako orchestrátor, alebo môžete všetko vytvoriť v Agent Service.

**Použitie**: Azure AI Agent Service je navrhnutý pre podnikové aplikácie, ktoré vyžadujú bezpečné, škálovateľné a flexibilné nasadenie AI agentov.

## Aký je rozdiel medzi týmito rámcami?

Zdá sa, že medzi týmito rámcami je veľa prekrytia, ale existujú kľúčové rozdiely v ich dizajne, schopnostiach a cieľových prípadoch použitia:

- **AutoGen**: Je experimentálny rámec zameraný na špičkový výskum multi-agentových systémov. Je najlepším miestom na experimentovanie a prototypovanie sofistikovaných multi-agentových systémov.
- **Semantic Kernel**: Je produkčne pripravená knižnica agentov na tvorbu podnikových agentických aplikácií. Zameriava sa na aplikácie riadené udalosťami, distribuované agentické aplikácie, umožňujúce viac LLMs a SLMs, nástroje a návrhové vzory pre jedného alebo viacerých agentov.
- **Azure AI Agent Service**: Je platforma a služba nasadenia v Azure Foundry pre agentov. Ponúka budovanie konektivity k službám podporovaným Azure, ako sú Azure OpenAI, Azure AI Search, Bing Search a vykonávanie kódu.

Stále si nie ste istí, ktorý si vybrať?

### Použitie

Pozrime sa, či vám môžeme pomôcť prejsť niektoré bežné prípady použitia:

> Otázka: Experimentujem, učím sa a vytváram proof-of-concept aplikácie agentov a chcem rýchlo budovať a experimentovať.

> Odpoveď: AutoGen by bol dobrý výber pre tento scenár, pretože sa zameriava na aplikácie riadené udalosťami, distribuované agentické aplikácie a podporuje pokročilé návrhové vzory pre multi-agentov.

> Otázka: Čo robí AutoGen lepšou voľbou ako Semantic Kernel a Azure AI Agent Service pre tento prípad použitia?

> Odpoveď: AutoGen je špeciálne navrhnutý pre aplikácie riadené udalosťami, distribuované agentické aplikácie, čo ho robí vhodným na automatizáciu úloh generovania kódu a analýzy dát. Poskytuje potrebné nástroje a schopnosti na efektívne budovanie komplexných multi-agentových systémov.

> Otázka: Znie to, že Azure AI Agent Service by tu tiež mohol fungovať, má nástroje na generovanie kódu a viac?

> Odpoveď: Áno, Azure AI Agent Service je platformová služba pre agentov a pridáva zabudované schopnosti pre viaceré modely, Azure AI Search, Bing Search a Azure Functions. Umožňuje ľahko vytvárať vašich agentov v Foundry Portáli a nasadiť ich vo veľkom.

> Otázka: Stále som zmätený, dajte mi len jednu možnosť.

> Odpoveď: Skvelou voľbou je najprv vytvoriť vašu aplikáciu v Semantic Kernel a potom použiť Azure AI Agent Service na nasadenie vášho agenta. Tento prístup vám umožňuje ľahko uchovávať vašich agentov a zároveň využívať silu na budovanie multi-agentových systémov v Semantic Kernel. Navyše, Semantic Kernel má konektor v AutoGen, čo uľahčuje používanie oboch rámcov spolu.

Zhrňme kľúčové rozdiely v tabuľke:

| Rámec | Zameranie | Základné koncepty | Použitie |
| --- | --- | --- | --- |
| AutoGen | Aplikácie riadené udalosťami, distribuované agentické aplikácie | Agenti, Persony, Funkcie, Dáta | Generovanie kódu, úlohy analýzy dát |
| Semantic Kernel | Porozumenie a generovanie textového obsahu podobného ľudskému | Agenti, Modulárne komponenty, Spolupráca | Porozumenie prirodzenému jazyku, generovanie obsahu |
| Azure AI Agent Service | Flexibilné modely, podniková bezpečnosť, Generovanie kódu, Volanie nástrojov | Modularita, Spolupráca, Orchestrácia procesov | Bezpečné, škálovateľné a flexibilné nasadenie AI agentov |

Aký je ideálny prípad použitia pre každý z týchto rámcov?

## Môžem priamo integrovať svoje existujúce nástroje Azure ekosystému, alebo potrebujem samostatné riešenia?

Odpoveď je áno, môžete priamo integrovať svoje existujúce nástroje Azure ekosystému s Azure AI Agent Service, najmä preto, že bol navrhnutý tak, aby bezproblémovo fungoval s inými službami Azure. Mohli by ste napríklad integrovať Bing, Azure AI Search a Azure Functions. Existuje tiež hlboká integrácia s Azure AI Foundry.

Pre AutoGen a Semantic Kernel môžete tiež integrovať s Azure službami, ale môže byť potrebné volať Azure služby z vášho kódu. Ďalším spôsobom integrácie je použitie Azure SDKs na interakciu s Azure službami z vašich agentov. Navyše, ako bolo spomenuté, môžete použiť Azure AI Agent Service ako orchestrátor pre vašich agentov vytvorených v AutoGen alebo Semantic Kernel, čo by poskytlo jednoduchý prístup k Azure ekosystému.

### Máte ďalšie otázky o AI Agent Frameworks?

Pripojte sa k [Azure AI Foundry Discord](https://aka.ms/ai-agents/discord), kde sa môžete stretnúť s ostatnými študentmi, zúčastniť sa konzultačných hodín a získať odpovede na vaše otázky o AI agentoch.

## Referencie

- ## Predchádzajúca lekcia

[Úvod do AI agentov a ich použitia](../01-intro-to-ai-agents/README.md)

## Nasledujúca lekcia

[Porozumenie návrhovým vzorom agentov](../03-agentic-design-patterns/README.md)

---

**Upozornenie**:  
Tento dokument bol preložený pomocou služby na automatický preklad [Co-op Translator](https://github.com/Azure/co-op-translator). Hoci sa snažíme o presnosť, upozorňujeme, že automatické preklady môžu obsahovať chyby alebo nepresnosti. Pôvodný dokument v jeho pôvodnom jazyku by mal byť považovaný za autoritatívny zdroj. Pre dôležité informácie sa odporúča profesionálny ľudský preklad. Nezodpovedáme za žiadne nedorozumenia alebo nesprávne interpretácie vyplývajúce z použitia tohto prekladu.