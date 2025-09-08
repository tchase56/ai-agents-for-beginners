<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-29T17:16:31+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "fi"
}
-->
[![Tutustu AI-agenttikehyksiin](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.fi.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(Klikkaa yllä olevaa kuvaa nähdäksesi tämän oppitunnin videon)_

# Tutustu AI-agenttikehyksiin

AI-agenttikehykset ovat ohjelmistoalustoja, jotka on suunniteltu helpottamaan AI-agenttien luomista, käyttöönottoa ja hallintaa. Nämä kehykset tarjoavat kehittäjille valmiita komponentteja, abstraktioita ja työkaluja, jotka yksinkertaistavat monimutkaisten AI-järjestelmien kehittämistä.

Nämä kehykset auttavat kehittäjiä keskittymään sovellustensa ainutlaatuisiin ominaisuuksiin tarjoamalla standardoituja lähestymistapoja AI-agenttien kehittämisen yleisiin haasteisiin. Ne parantavat skaalautuvuutta, saavutettavuutta ja tehokkuutta AI-järjestelmien rakentamisessa.

## Johdanto

Tämä oppitunti kattaa:

- Mitä AI-agenttikehykset ovat ja mitä ne mahdollistavat kehittäjille?
- Kuinka tiimit voivat käyttää näitä nopeasti prototyyppien luomiseen, iterointiin ja agenttien kyvykkyyksien parantamiseen?
- Mitkä ovat erot Microsoftin luomien kehysten ja työkalujen välillä?
- Voinko integroida olemassa olevat Azure-ekosysteemin työkalut suoraan, vai tarvitsenko erillisiä ratkaisuja?
- Mikä on Azure AI Agents -palvelu ja miten se auttaa minua?

## Oppimistavoitteet

Tämän oppitunnin tavoitteena on auttaa sinua ymmärtämään:

- AI-agenttikehysten rooli AI-kehityksessä.
- Kuinka hyödyntää AI-agenttikehyksiä älykkäiden agenttien rakentamiseen.
- AI-agenttikehysten mahdollistamat keskeiset kyvykkyydet.
- Erot AutoGenin, Semantic Kernelin ja Azure AI Agent Servicen välillä.

## Mitä AI-agenttikehykset ovat ja mitä ne mahdollistavat kehittäjille?

Perinteiset AI-kehykset voivat auttaa integroimaan tekoälyä sovelluksiin ja parantamaan näitä sovelluksia seuraavilla tavoilla:

- **Personointi**: Tekoäly voi analysoida käyttäjän käyttäytymistä ja mieltymyksiä tarjotakseen personoituja suosituksia, sisältöä ja kokemuksia.  
Esimerkki: Suoratoistopalvelut, kuten Netflix, käyttävät tekoälyä ehdottaakseen elokuvia ja ohjelmia katseluhistorian perusteella, mikä parantaa käyttäjän sitoutumista ja tyytyväisyyttä.

- **Automaatio ja tehokkuus**: Tekoäly voi automatisoida toistuvia tehtäviä, virtaviivaistaa työnkulkuja ja parantaa operatiivista tehokkuutta.  
Esimerkki: Asiakaspalvelusovellukset käyttävät tekoälyllä toimivia chatbotteja käsittelemään yleisiä kyselyitä, mikä lyhentää vastausaikoja ja vapauttaa ihmisiä monimutkaisempien ongelmien hoitamiseen.

- **Parannettu käyttökokemus**: Tekoäly voi parantaa kokonaisvaltaista käyttökokemusta tarjoamalla älykkäitä ominaisuuksia, kuten puheentunnistusta, luonnollisen kielen käsittelyä ja ennakoivaa tekstinsyöttöä.  
Esimerkki: Virtuaaliassistentit, kuten Siri ja Google Assistant, käyttävät tekoälyä ymmärtääkseen ja vastatakseen puhekomentoihin, mikä helpottaa käyttäjien vuorovaikutusta laitteidensa kanssa.

### Kuulostaa hyvältä, eikö? Miksi tarvitsemme AI-agenttikehyksen?

AI-agenttikehykset edustavat jotain enemmän kuin pelkät AI-kehykset. Ne on suunniteltu mahdollistamaan älykkäiden agenttien luominen, jotka voivat olla vuorovaikutuksessa käyttäjien, muiden agenttien ja ympäristön kanssa saavuttaakseen tiettyjä tavoitteita. Nämä agentit voivat osoittaa autonomista käyttäytymistä, tehdä päätöksiä ja sopeutua muuttuviin olosuhteisiin. Katsotaanpa joitakin AI-agenttikehysten mahdollistamia keskeisiä kyvykkyyksiä:

- **Agenttien yhteistyö ja koordinointi**: Mahdollistaa useiden AI-agenttien luomisen, jotka voivat työskennellä yhdessä, kommunikoida ja koordinoida ratkaistakseen monimutkaisia tehtäviä.
- **Tehtävien automaatio ja hallinta**: Tarjoaa mekanismeja monivaiheisten työnkulkujen automatisointiin, tehtävien delegointiin ja dynaamiseen tehtävien hallintaan agenttien kesken.
- **Kontekstin ymmärtäminen ja sopeutuminen**: Varustaa agentit kyvyllä ymmärtää konteksti, sopeutua muuttuviin ympäristöihin ja tehdä päätöksiä reaaliaikaisen tiedon perusteella.

Yhteenvetona voidaan todeta, että agentit mahdollistavat enemmän, vievät automaation seuraavalle tasolle ja luovat älykkäämpiä järjestelmiä, jotka voivat sopeutua ja oppia ympäristöstään.

## Kuinka nopeasti prototyyppien luominen, iterointi ja agenttien kyvykkyyksien parantaminen onnistuu?

Tämä on nopeasti kehittyvä ala, mutta on olemassa joitakin yhteisiä piirteitä useimmissa AI-agenttikehyksissä, jotka voivat auttaa sinua nopeasti prototyyppien luomisessa ja iteroinnissa, kuten modulaariset komponentit, yhteistyötyökalut ja reaaliaikainen oppiminen. Sukelletaan näihin:

- **Käytä modulaarisia komponentteja**: AI-SDK:t tarjoavat valmiita komponentteja, kuten AI- ja muistiliittimiä, luonnollisen kielen tai koodipluginien avulla tapahtuvaa funktiokutsua, kehotemalleja ja paljon muuta.
- **Hyödynnä yhteistyötyökaluja**: Suunnittele agentteja, joilla on erityiset roolit ja tehtävät, mikä mahdollistaa yhteistyötyönkulkujen testaamisen ja parantamisen.
- **Opi reaaliajassa**: Toteuta palautesilmukoita, joissa agentit oppivat vuorovaikutuksista ja mukauttavat käyttäytymistään dynaamisesti.

### Käytä modulaarisia komponentteja

SDK:t, kuten Microsoft Semantic Kernel ja LangChain, tarjoavat valmiita komponentteja, kuten AI-liittimiä, kehotemalleja ja muistinhallintaa.

**Kuinka tiimit voivat käyttää näitä**: Tiimit voivat nopeasti koota nämä komponentit toimivan prototyypin luomiseksi ilman, että heidän tarvitsee aloittaa tyhjästä, mikä mahdollistaa nopean kokeilun ja iteroinnin.

**Kuinka tämä toimii käytännössä**: Voit käyttää valmiiksi rakennettua parseria käyttäjän syötteen tiedon eristämiseen, muistimoduulia tietojen tallentamiseen ja hakemiseen sekä kehotegeneraattoria vuorovaikutukseen käyttäjien kanssa, kaikki ilman näiden komponenttien rakentamista alusta alkaen.

**Esimerkkikoodi**. Katsotaanpa esimerkkejä siitä, kuinka voit käyttää valmiiksi rakennettua AI-liitintä Semantic Kernel Pythonilla ja .Netillä, joka käyttää automaattista funktiokutsua mallin vastaamiseen käyttäjän syötteeseen:

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

Tässä esimerkissä näet, kuinka voit hyödyntää valmiiksi rakennettua parseria käyttäjän syötteen keskeisten tietojen, kuten lähtöpaikan, määränpään ja päivämäärän, eristämiseen lentovarauksen pyynnöstä. Tämä modulaarinen lähestymistapa mahdollistaa keskittymisen korkean tason logiikkaan.

### Hyödynnä yhteistyötyökaluja

Kehykset, kuten CrewAI, Microsoft AutoGen ja Semantic Kernel, helpottavat useiden agenttien luomista, jotka voivat työskennellä yhdessä.

**Kuinka tiimit voivat käyttää näitä**: Tiimit voivat suunnitella agentteja, joilla on erityiset roolit ja tehtävät, mikä mahdollistaa yhteistyötyönkulkujen testaamisen ja parantamisen sekä järjestelmän tehokkuuden parantamisen.

**Kuinka tämä toimii käytännössä**: Voit luoda agenttitiimin, jossa jokaisella agentilla on erikoistunut tehtävä, kuten tiedonhaku, analyysi tai päätöksenteko. Nämä agentit voivat kommunikoida ja jakaa tietoa saavuttaakseen yhteisen tavoitteen, kuten käyttäjän kyselyyn vastaamisen tai tehtävän suorittamisen.

**Esimerkkikoodi (AutoGen)**:

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

Edellisessä koodissa näet, kuinka voit luoda tehtävän, joka sisältää useita agentteja, jotka työskentelevät yhdessä analysoidakseen tietoja. Jokainen agentti suorittaa tietyn tehtävän, ja tehtävä toteutetaan koordinoimalla agenttien toimintaa halutun lopputuloksen saavuttamiseksi. Luomalla erikoistuneita agentteja voit parantaa tehtävän tehokkuutta ja suorituskykyä.

### Opi reaaliajassa

Edistyneet kehykset tarjoavat kyvykkyyksiä reaaliaikaiseen kontekstin ymmärtämiseen ja sopeutumiseen.

**Kuinka tiimit voivat käyttää näitä**: Tiimit voivat toteuttaa palautesilmukoita, joissa agentit oppivat vuorovaikutuksista ja mukauttavat käyttäytymistään dynaamisesti, mikä johtaa jatkuvaan parantamiseen ja kyvykkyyksien hienosäätöön.

**Kuinka tämä toimii käytännössä**: Agentit voivat analysoida käyttäjäpalautetta, ympäristötietoja ja tehtävän tuloksia päivittääkseen tietokantaansa, mukauttaakseen päätöksentekoalgoritmejaan ja parantaakseen suorituskykyään ajan myötä. Tämä iteratiivinen oppimisprosessi mahdollistaa agenttien sopeutumisen muuttuviin olosuhteisiin ja käyttäjien mieltymyksiin, mikä parantaa järjestelmän kokonaistehokkuutta.

## Mitkä ovat erot AutoGenin, Semantic Kernelin ja Azure AI Agent Servicen välillä?

Näitä kehyksiä voidaan verrata monin tavoin, mutta tarkastellaan joitakin keskeisiä eroja niiden suunnittelussa, kyvykkyyksissä ja kohdekäyttötapauksissa:

## AutoGen

AutoGen on Microsoft Researchin AI Frontiers Labin kehittämä avoimen lähdekoodin kehys. Se keskittyy tapahtumapohjaisiin, hajautettuihin *agenttisiin* sovelluksiin, jotka mahdollistavat useiden LLM:ien ja SLM:ien, työkalujen ja edistyneiden monen agentin suunnittelumallien käytön.

AutoGen perustuu agenttien ydinajatukseen, jotka ovat autonomisia yksiköitä, jotka voivat havaita ympäristönsä, tehdä päätöksiä ja ryhtyä toimiin saavuttaakseen tiettyjä tavoitteita. Agentit kommunikoivat asynkronisten viestien kautta, mikä mahdollistaa niiden itsenäisen ja rinnakkaisen työskentelyn, parantaen järjestelmän skaalautuvuutta ja reagointikykyä.

Wikipedia määrittelee näyttelijän (actor) seuraavasti: _"Perusosa rinnakkaislaskennassa. Vastauksena vastaanottamaansa viestiin näyttelijä voi: tehdä paikallisia päätöksiä, luoda lisää näyttelijöitä, lähettää lisää viestejä ja päättää, miten vastata seuraavaan vastaanotettuun viestiin."_  

**Käyttötapaukset**: Koodin automaattinen generointi, data-analyysitehtävät ja räätälöityjen agenttien rakentaminen suunnittelu- ja tutkimustoimintoihin.

Tässä ovat AutoGenin tärkeät ydinajatukset:

- **Agentit**. Agentti on ohjelmistoyksikkö, joka:  
  - **Kommunikoi viestien kautta**, jotka voivat olla synkronisia tai asynkronisia.  
  - **Ylläpitää omaa tilaansa**, jota saapuvat viestit voivat muuttaa.  
  - **Suorittaa toimia** vastauksena vastaanotettuihin viesteihin tai tilansa muutoksiin. Nämä toimet voivat muuttaa agentin tilaa ja tuottaa ulkoisia vaikutuksia, kuten viestilokien päivittämistä, uusien viestien lähettämistä, koodin suorittamista tai API-kutsujen tekemistä.  

  Tässä on lyhyt koodiesimerkki, jossa luot oman agentin chat-ominaisuuksilla:

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

    Edellisessä koodissa on luotu `MyAssistant`, joka perii `RoutedAgent`-luokan. Sillä on viestinkäsittelijä, joka tulostaa viestin sisällön ja lähettää sitten vastauksen `AssistantAgent`-deleegaatin avulla. Huomaa erityisesti, kuinka `self._delegate`-muuttujalle annetaan `AssistantAgent`-instanssi, joka on valmiiksi rakennettu agentti, joka voi käsitellä chat-vastauksia.

    Seuraavaksi ilmoitetaan AutoGenille tästä agenttityypistä ja käynnistetään ohjelma:

    ```python
    
    # main.py
    runtime = SingleThreadedAgentRuntime()
    await MyAgent.register(runtime, "my_agent", lambda: MyAgent())

    runtime.start()  # Start processing messages in the background.
    await runtime.send_message(MyMessageType("Hello, World!"), AgentId("my_agent", "default"))
    ```  

    Edellisessä koodissa agentit rekisteröidään ajonaikaisessa ympäristössä, ja sitten agentille lähetetään viesti, mikä tuottaa seuraavan tuloksen:

    ```text
    # Output from the console:
    my_agent received message: Hello, World!
    my_assistant received message: Hello, World!
    my_assistant responded: Hello! How can I assist you today?
    ```  

- **Moniagenttisuus**. AutoGen tukee useiden agenttien luomista, jotka voivat työskennellä yhdessä saavuttaakseen monimutkaisia tehtäviä. Agentit voivat kommunikoida, jakaa tietoa ja koordinoida toimiaan ongelmien ratkaisemiseksi tehokkaammin. Moniagenttijärjestelmän luomiseksi voit määritellä erilaisia agenttityyppejä, joilla on erikoistuneet toiminnot ja roolit, kuten tiedonhaku, analyysi, päätöksenteko ja käyttäjävuorovaikutus. Katsotaanpa, miltä tällainen luominen näyttää:

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

    Edellisessä koodissa on `GroupChatManager`, joka rekisteröidään ajonaikaisessa ympäristössä. Tämä manageri vastaa eri agenttityyppien, kuten kirjoittajien, kuvittajien, toimittajien ja käyttäjien, vuorovaikutuksen koordinoinnista.

- **Agenttien ajonaikainen ympäristö**. Kehys tarjoaa ajonaikaisen ympäristön, joka mahdollistaa agenttien välisen viestinnän, hallitsee niiden identiteettejä ja elinkaaria sekä varmistaa turvallisuus- ja yksityisyysrajat. Tämä tarkoittaa, että voit ajaa agenttejasi turvallisessa ja hallitussa ympäristössä, mikä varmistaa niiden turvallisen ja tehokkaan vuorovaikutuksen. Kiinnostavia ajonaikaisia ympäristöjä on kaksi:  
  - **Itsenäinen ajonaikainen ympäristö**. Tämä on hyvä valinta yksiprosessisovelluksille, joissa kaikki agentit on toteutettu samalla ohjelmointikielellä ja ne toimivat samassa prosessissa. Tässä on havainnollistus siitä, miten se toimii:  

    Sovelluspino  

    *agentit kommunikoivat viestien kautta ajonaikaisessa ympäristössä, joka hallitsee agenttien elinkaarta*  

  - **Hajautettu agenttien ajonaikainen ympäristö**, joka sopii moniprosessisovelluksille, joissa agentit voivat olla toteutettu eri ohjelmointikielillä ja toimia eri koneilla. Tässä on havainnollistus siitä, miten se toimii:  

## Semantic Kernel + Agent Framework

Semantic Kernel on yritysvalmis AI Orchestration SDK. Se koostuu AI- ja muistiliittimistä sekä Agent Frameworkista.

Käsitellään ensin joitakin keskeisiä komponentteja:

- **AI-liittimet**: Tämä on rajapinta ulkoisiin AI-palveluihin ja tietolähteisiin, joita voidaan käyttää sekä Pythonilla että C#:lla.

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

    Tässä on yksinkertainen esimerkki siitä, kuinka voit luoda kernelin ja lisätä chat-vastauspalvelun. Semantic Kernel luo yhteyden ulkoiseen AI-palveluun, tässä tapauksessa Azure OpenAI Chat Completioniin.

- **Pluginit**: Nämä kapseloivat toimintoja, joita sovellus voi käyttää. On olemassa sekä valmiita plugineja että räätälöityjä, joita voit luoda. Liittyvä käsite on "kehotefunktiot". Sen sijaan, että tarjoaisit luonnollisen kielen vihjeitä funktiokutsuille, lähetät tiettyjä funktioita mallille. Nykyisen chat-kontekstin perusteella malli voi valita kutsua jonkin näistä funktioista pyynnön tai kyselyn suorittamiseksi. Tässä on esimerkki:

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

    Tässä sinulla on ensin kehotemalli `skPrompt`, joka jättää tilaa käyttäjän syötteelle, `$userInput`. Sitten luot kernel-funktion `SummarizeText` ja viet sen kerneliin plugin-nimellä `SemanticFunctions`. Huomaa funktion nimi, joka auttaa Semantic Kernelia ymmärtämään, mitä funktio tekee ja milloin sitä
## Azure AI Agent Service

Azure AI Agent Service on uudempi lisäys, joka esiteltiin Microsoft Ignite 2024 -tapahtumassa. Se mahdollistaa AI-agenttien kehittämisen ja käyttöönoton joustavammilla malleilla, kuten avoimen lähdekoodin LLM-mallien (esim. Llama 3, Mistral ja Cohere) suoralla kutsumisella.

Azure AI Agent Service tarjoaa vahvempia yritystason tietoturvamekanismeja ja tietojen tallennusmenetelmiä, mikä tekee siitä sopivan yrityssovelluksiin.

Se toimii heti valmiina monen agentin orkestrointikehysten, kuten AutoGenin ja Semantic Kernelin, kanssa.

Tämä palvelu on tällä hetkellä julkisessa esikatselussa ja tukee Pythonia ja C#:a agenttien rakentamiseen.

Käyttämällä Semantic Kernel Pythonia voimme luoda Azure AI Agentin käyttäjän määrittelemällä liitännäisellä:

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

### Keskeiset käsitteet

Azure AI Agent Servicellä on seuraavat keskeiset käsitteet:

- **Agentti**. Azure AI Agent Service integroituu Azure AI Foundryyn. AI Foundryssa AI-agentti toimii "älykkäänä" mikropalveluna, jota voidaan käyttää kysymyksiin vastaamiseen (RAG), toimintojen suorittamiseen tai työnkulkujen täydelliseen automatisointiin. Tämä saavutetaan yhdistämällä generatiivisten AI-mallien voima työkaluihin, jotka mahdollistavat pääsyn ja vuorovaikutuksen todellisten tietolähteiden kanssa. Tässä esimerkki agentista:

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    Tässä esimerkissä luodaan agentti mallilla `gpt-4o-mini`, nimellä `my-agent` ja ohjeilla `You are helpful agent`. Agentti on varustettu työkaluilla ja resursseilla koodin tulkintatehtävien suorittamiseen.

- **Keskusteluketju ja viestit**. Keskusteluketju on toinen tärkeä käsite. Se edustaa keskustelua tai vuorovaikutusta agentin ja käyttäjän välillä. Keskusteluketjuja voidaan käyttää keskustelun etenemisen seuraamiseen, kontekstin tallentamiseen ja vuorovaikutuksen tilan hallintaan. Tässä esimerkki keskusteluketjusta:

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

    Edellisessä koodissa luodaan keskusteluketju. Tämän jälkeen ketjuun lähetetään viesti. Kutsumalla `create_and_process_run` agenttia pyydetään suorittamaan tehtävä keskusteluketjussa. Lopuksi viestit haetaan ja kirjataan agentin vastauksen tarkastelemiseksi. Viestit osoittavat keskustelun etenemisen käyttäjän ja agentin välillä. On myös tärkeää ymmärtää, että viestit voivat olla eri tyyppisiä, kuten tekstiä, kuvia tai tiedostoja, eli agentin työ voi johtaa esimerkiksi kuvaan tai tekstivastaukseen. Kehittäjänä voit käyttää tätä tietoa vastauksen jatkokäsittelyyn tai sen esittämiseen käyttäjälle.

- **Integroituu muihin AI-kehyksiin**. Azure AI Agent Service voi olla vuorovaikutuksessa muiden kehysten, kuten AutoGenin ja Semantic Kernelin, kanssa. Tämä tarkoittaa, että voit rakentaa osan sovelluksestasi jossakin näistä kehyksistä ja käyttää esimerkiksi Agent Serviceä orkestroijana tai rakentaa kaiken Agent Servicen avulla.

**Käyttötapaukset**: Azure AI Agent Service on suunniteltu yrityssovelluksiin, jotka vaativat turvallista, skaalautuvaa ja joustavaa AI-agenttien käyttöönottoa.

## Mitä eroa näillä kehyksillä on?

Vaikuttaa siltä, että näissä kehyksissä on paljon päällekkäisyyksiä, mutta niiden suunnittelussa, ominaisuuksissa ja kohdekäyttötapauksissa on joitakin keskeisiä eroja:

- **AutoGen**: On kokeilukehys, joka keskittyy huippututkimukseen monen agentin järjestelmistä. Se on paras paikka kokeilla ja prototyyppien rakentamiseen kehittyneille monen agentin järjestelmille.
- **Semantic Kernel**: On tuotantovalmis agenttikirjasto yritystason agenttisovellusten rakentamiseen. Se keskittyy tapahtumapohjaisiin, hajautettuihin agenttisovelluksiin, jotka mahdollistavat useiden LLM- ja SLM-mallien, työkalujen sekä yhden/monta-agentin suunnittelumallien käytön.
- **Azure AI Agent Service**: On Azure Foundryssa toimiva alusta ja käyttöönottopalvelu agenteille. Se tarjoaa yhteyden rakentamisen Azure Foundryn tukemiin palveluihin, kuten Azure OpenAI, Azure AI Search, Bing Search ja koodin suoritus.

Etkö ole vieläkään varma, minkä valita?

### Käyttötapaukset

Katsotaanpa, voimmeko auttaa sinua käymällä läpi joitakin yleisiä käyttötapauksia:

> K: Kokeilen, opettelen ja rakennan todisteita konseptista agenttisovelluksille, ja haluan pystyä rakentamaan ja kokeilemaan nopeasti
>

> V: AutoGen olisi hyvä valinta tähän tilanteeseen, koska se keskittyy tapahtumapohjaisiin, hajautettuihin agenttisovelluksiin ja tukee kehittyneitä monen agentin suunnittelumalleja.

> K: Mikä tekee AutoGenistä paremman valinnan kuin Semantic Kernel ja Azure AI Agent Service tähän käyttötapaukseen?
>
> V: AutoGen on erityisesti suunniteltu tapahtumapohjaisiin, hajautettuihin agenttisovelluksiin, mikä tekee siitä hyvin sopivan koodin generointiin ja data-analyysitehtäviin. Se tarjoaa tarvittavat työkalut ja ominaisuudet monimutkaisten monen agentin järjestelmien rakentamiseen tehokkaasti.

> K: Kuulostaa siltä, että Azure AI Agent Service voisi toimia tässä myös, sillä siinä on työkaluja koodin generointiin ja muuhun?
>
> V: Kyllä, Azure AI Agent Service on agenttialustapalvelu, joka sisältää sisäänrakennettuja ominaisuuksia useille malleille, Azure AI Searchille, Bing Searchille ja Azure Functionsille. Se tekee agenttien rakentamisesta helppoa Foundry-portaalissa ja niiden käyttöönotosta skaalautuvaa.

> K: Olen edelleen hämmentynyt, anna vain yksi vaihtoehto
>
> V: Erinomainen valinta on rakentaa sovelluksesi ensin Semantic Kernelissä ja käyttää sitten Azure AI Agent Serviceä agenttisi käyttöönottoon. Tämä lähestymistapa mahdollistaa agenttien helpon säilyttämisen samalla, kun hyödynnetään Semantic Kernelin voimaa monen agentin järjestelmien rakentamiseen. Lisäksi Semantic Kernelillä on liitin AutoGeniin, mikä tekee molempien kehysten käytöstä yhdessä helppoa.

Tiivistetään tärkeimmät erot taulukkoon:

| Kehys | Painopiste | Keskeiset käsitteet | Käyttötapaukset |
| --- | --- | --- | --- |
| AutoGen | Tapahtumapohjaiset, hajautetut agenttisovellukset | Agentit, Persoonat, Funktiot, Data | Koodin generointi, data-analyysitehtävät |
| Semantic Kernel | Ihmismäisen tekstisisällön ymmärtäminen ja generointi | Agentit, Modulaariset komponentit, Yhteistyö | Luonnollisen kielen ymmärtäminen, sisällön generointi |
| Azure AI Agent Service | Joustavat mallit, yritystason tietoturva, Koodin generointi, Työkalujen kutsuminen | Modulaarisuus, Yhteistyö, Prosessien orkestrointi | Turvallinen, skaalautuva ja joustava AI-agenttien käyttöönotto |

Mikä on ihanteellinen käyttötapaus kullekin näistä kehyksistä?

## Voinko integroida olemassa olevat Azure-ekosysteemin työkaluni suoraan vai tarvitsenko erillisiä ratkaisuja?

Vastaus on kyllä, voit integroida olemassa olevat Azure-ekosysteemin työkalusi suoraan erityisesti Azure AI Agent Servicen kanssa, koska se on rakennettu toimimaan saumattomasti muiden Azure-palveluiden kanssa. Voit esimerkiksi integroida Bingin, Azure AI Searchin ja Azure Functionsin. Lisäksi siinä on syvä integraatio Azure AI Foundryn kanssa.

AutoGenin ja Semantic Kernelin kanssa voit myös integroida Azure-palveluita, mutta se saattaa vaatia Azure-palveluiden kutsumista koodistasi. Toinen tapa integroida on käyttää Azure SDK:ita vuorovaikutukseen Azure-palveluiden kanssa agenteistasi. Lisäksi, kuten mainittiin, voit käyttää Azure AI Agent Serviceä orkestroijana AutoGenissä tai Semantic Kernelissä rakennetuissa agenteissasi, mikä mahdollistaa helpon pääsyn Azure-ekosysteemiin.

### Onko sinulla lisää kysymyksiä AI-agenttikehyksistä?

Liity [Azure AI Foundry Discordiin](https://aka.ms/ai-agents/discord) tapaamaan muita oppijoita, osallistumaan toimistoaikoihin ja saamaan vastauksia AI-agentteihin liittyviin kysymyksiisi.

## Viitteet

- 

## Edellinen oppitunti

[Johdanto AI-agentteihin ja käyttötapauksiin](../01-intro-to-ai-agents/README.md)

## Seuraava oppitunti

[Agenttisuunnittelumallien ymmärtäminen](../03-agentic-design-patterns/README.md)

---

**Vastuuvapauslauseke**:  
Tämä asiakirja on käännetty käyttämällä tekoälypohjaista käännöspalvelua [Co-op Translator](https://github.com/Azure/co-op-translator). Pyrimme tarkkuuteen, mutta huomioithan, että automaattiset käännökset voivat sisältää virheitä tai epätarkkuuksia. Alkuperäistä asiakirjaa sen alkuperäisellä kielellä tulee pitää ensisijaisena lähteenä. Kriittisen tiedon osalta suositellaan ammattimaista ihmiskääntämistä. Emme ole vastuussa tämän käännöksen käytöstä aiheutuvista väärinkäsityksistä tai virhetulkinnoista.