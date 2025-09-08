<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-30T00:02:50+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "my"
}
-->
[![AI Agent Frameworks ကို ရှာဖွေခြင်း](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.my.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(ဤသင်ခန်းစာ၏ ဗီဒီယိုကို ကြည့်ရန် အထက်ပါ ပုံကို နှိပ်ပါ)_

# AI Agent Frameworks ကို ရှာဖွေခြင်း

AI agent frameworks ဆိုသည်မှာ AI agent များကို ဖန်တီးခြင်း၊ တင်သွင်းခြင်းနှင့် စီမံခန့်ခွဲခြင်းကို လွယ်ကူစေသော ဆော့ဖ်ဝဲပလက်ဖောင်းများဖြစ်သည်။ ဤ frameworks များသည် developer များအတွက် အဆင့်မြင့် AI စနစ်များ ဖွံ့ဖြိုးတိုးတက်စေရန် အဆင့်မြင့် component များ၊ abstraction များနှင့် tools များကို ပေးစွမ်းသည်။

ဤ frameworks များသည် AI agent ဖွံ့ဖြိုးတိုးတက်မှုတွင် ရှေ့ဆောင်သော စိန်ခေါ်မှုများအတွက် စံပြနည်းလမ်းများကို ပေးစွမ်းခြင်းအားဖြင့် application များ၏ ထူးခြားသော အပိုင်းများကို developer များအာရုံစိုက်နိုင်စေသည်။ AI စနစ်များကို တိုးတက်မှု၊ လွယ်ကူမှုနှင့် ထိရောက်မှုရှိစေရန် အထောက်အကူပြုသည်။

## အကျဉ်းချုပ်

ဤသင်ခန်းစာတွင် အောက်ပါအကြောင်းအရာများကို လေ့လာမည်-

- AI Agent Frameworks ဆိုတာဘာလဲ၊ developer များအတွက် ဘာတွေကို လုပ်ဆောင်နိုင်စေသလဲ?
- အဖွဲ့များသည် ဤ frameworks များကို အသုံးပြု၍ agent ၏ စွမ်းရည်များကို prototype လုပ်ခြင်း၊ iteration လုပ်ခြင်းနှင့် တိုးတက်စေရန် ဘယ်လို အသုံးချနိုင်မလဲ?
- Microsoft မှ ဖန်တီးထားသော frameworks နှင့် tools များအကြား ကွာခြားချက်များက ဘာလဲ?
- Azure ecosystem tools များကို တိုက်ရိုက် ပေါင်းစည်းနိုင်မလား၊ သို့မဟုတ် standalone solutions များလိုအပ်ပါသလား?
- Azure AI Agents service ဆိုတာဘာလဲ၊ ဒါက ကျွန်တော်/ကျွန်မကို ဘယ်လို အထောက်အကူပေးနိုင်မလဲ?

## သင်ယူရမည့် ရည်မှန်းချက်များ

ဤသင်ခန်းစာ၏ ရည်မှန်းချက်များမှာ-

- AI Agent Frameworks ၏ AI ဖွံ့ဖြိုးတိုးတက်မှုတွင် ပါဝင်မှုကို နားလည်စေရန်။
- AI Agent Frameworks ကို အသုံးပြု၍ ဉာဏ်ရည်ရှိသော agent များ ဖန်တီးနိုင်ရန်။
- AI Agent Frameworks မှ ပေးစွမ်းသော အဓိကစွမ်းရည်များကို နားလည်ရန်။
- AutoGen, Semantic Kernel နှင့် Azure AI Agent Service တို့၏ ကွာခြားချက်များကို နားလည်ရန်။

## AI Agent Frameworks ဆိုတာဘာလဲ၊ developer များအတွက် ဘာတွေကို လုပ်ဆောင်နိုင်စေသလဲ?

ရိုးရာ AI Frameworks များသည် AI ကို app များတွင် ပေါင်းစည်းခြင်းနှင့် app များကို အောက်ပါနည်းလမ်းများဖြင့် ပိုမိုကောင်းမွန်စေရန် အထောက်အကူပေးနိုင်သည်-

- **Personalization**: AI သည် user ၏ အပြုအမူနှင့် အကြိုက်အရွေးများကို ခွဲခြားလေ့လာပြီး အကြံပြုချက်များ၊ အကြောင်းအရာများနှင့် အတွေ့အကြုံများကို တိုင်းတာပေးနိုင်သည်။
ဥပမာ- Netflix ကဲ့သို့သော streaming services များသည် AI ကို အသုံးပြု၍ ကြည့်ရှုမှုမှတ်တမ်းအပေါ် အခြေခံပြီး ရုပ်ရှင်နှင့် ရုပ်သံအစီအစဉ်များကို အကြံပြုပေးသည်။

- **Automation နှင့် ထိရောက်မှု**: AI သည် ထပ်တလဲလဲလုပ်ဆောင်ရသော အလုပ်များကို အလိုအလျောက်လုပ်ဆောင်ခြင်း၊ workflow များကို streamline လုပ်ခြင်းနှင့် စီမံခန့်ခွဲမှုထိရောက်မှုကို တိုးတက်စေသည်။
ဥပမာ- Customer service apps များသည် AI-powered chatbots ကို အသုံးပြု၍ အများဆုံးမေးခွန်းများကို ဖြေကြားပေးခြင်း၊ အချိန်ကုန်ကျမှုကို လျှော့ချခြင်းနှင့် လူ့ agent များကို ပိုမိုရှုပ်ထွေးသော အကြောင်းအရာများအတွက် အချိန်ပေးနိုင်စေသည်။

- **User Experience တိုးတက်မှု**: AI သည် အသံသိရှိမှု၊ သဘာဝဘာသာစကားကို နားလည်ခြင်းနှင့် အကြိုတင်စာသားခန့်မှန်းခြင်းကဲ့သို့သော ဉာဏ်ရည်ရှိသော feature များကို ပေးစွမ်းခြင်းအားဖြင့် user experience ကို တိုးတက်စေသည်။
ဥပမာ- Siri နှင့် Google Assistant ကဲ့သို့သော virtual assistants များသည် အသံအမိန့်များကို နားလည်ပြီး တုံ့ပြန်ပေးရန် AI ကို အသုံးပြုသည်။

### ဒါတွေကောင်းတယ်လို့ ထင်ရတယ်၊ ဒါပေမယ့် AI Agent Framework ဘာကြောင့် လိုအပ်သလဲ?

AI Agent frameworks သည် ရိုးရိုး AI frameworks ထက် ပိုမိုတိုးတက်သော အရာတစ်ခုကို ကိုယ်စားပြုသည်။ ၎င်းတို့သည် user များ၊ အခြား agent များနှင့် ပတ်ဝန်းကျင်တို့နှင့် အပြန်အလှန်ဆက်သွယ်နိုင်သော ဉာဏ်ရည်ရှိသော agent များကို ဖန်တီးရန်အတွက် ဖန်တီးထားသည်။ Agent များသည် အလိုအလျောက်အပြုအမူကို ပြသနိုင်ပြီး ဆုံးဖြတ်ချက်များကို ချမှတ်နိုင်သည်။ AI Agent Frameworks မှ ပေးစွမ်းသော အဓိကစွမ်းရည်များကို ကြည့်ကြရအောင်-

- **Agent Collaboration နှင့် Coordination**: Agent များအချင်းချင်း ပေါင်းစည်းဆောင်ရွက်ခြင်း၊ ဆက်သွယ်ခြင်းနှင့် ရှုပ်ထွေးသော အလုပ်များကို ဖြေရှင်းရန် ပေါင်းစည်းလုပ်ဆောင်နိုင်စေသည်။
- **Task Automation နှင့် Management**: Multi-step workflows များကို အလိုအလျောက်လုပ်ဆောင်ခြင်း၊ task များကို အပ်နှံခြင်းနှင့် agent များအကြား dynamic task management ကို ပံ့ပိုးပေးသည်။
- **Contextual Understanding နှင့် Adaptation**: Agent များကို ပတ်ဝန်းကျင်ကို နားလည်နိုင်စေခြင်း၊ အခြေအနေများပြောင်းလဲမှုကို လိုက်လျောညီထွေဖြစ်စေခြင်းနှင့် အချိန်နှင့်တပြေးညီ အချက်အလက်များအပေါ် အခြေခံ၍ ဆုံးဖြတ်ချက်ချနိုင်စေသည်။

အကျဉ်းချုပ်အားဖြင့် agent များသည် automation ကို နောက်တစ်ဆင့်တိုးတက်စေပြီး ပတ်ဝန်းကျင်မှ သင်ယူနိုင်သော ပိုမိုဉာဏ်ရည်ရှိသော စနစ်များကို ဖန်တီးနိုင်စေသည်။

## Agent ၏ စွမ်းရည်များကို prototype လုပ်ခြင်း၊ iteration လုပ်ခြင်းနှင့် တိုးတက်စေရန် ဘယ်လို လျင်မြန်စွာ လုပ်ဆောင်နိုင်မလဲ?

AI Agent Frameworks များတွင် module components, collaborative tools, real-time learning ကဲ့သို့သော အခြေခံအချက်များကို အသုံးပြု၍ prototype လုပ်ခြင်းနှင့် iteration လုပ်ခြင်းကို လျင်မြန်စွာ လုပ်ဆောင်နိုင်သည်။ 

- **Modular Components ကို အသုံးပြုပါ**: AI SDKs တွင် AI နှင့် Memory connectors, natural language သို့မဟုတ် code plugins အသုံးပြုသော function calling, prompt templates စသည်တို့ကဲ့သို့သော pre-built components များပါဝင်သည်။
- **Collaborative Tools ကို အသုံးချပါ**: အထူးသတ်မှတ်ထားသော အခန်းကဏ္ဍများနှင့် အလုပ်များဖြင့် agent များကို ဒီဇိုင်းဆွဲခြင်း၊ collaborative workflows များကို စမ်းသပ်ခြင်းနှင့် တိုးတက်စေရန်။
- **Real-Time Learning ကို အကောင်အထည်ဖော်ပါ**: Agent များသည် အပြန်အလှန်ဆက်သွယ်မှုများမှ သင်ယူပြီး ၎င်းတို့၏ အပြုအမူကို dynamic အနေဖြင့် ပြင်ဆင်နိုင်သော feedback loops များကို အကောင်အထည်ဖော်ပါ။

### Modular Components ကို အသုံးပြုခြင်း

Microsoft Semantic Kernel နှင့် LangChain ကဲ့သို့သော SDKs တွင် AI connectors, prompt templates, memory management ကဲ့သို့သော pre-built components များပါဝင်သည်။

**အဖွဲ့များသည် ဤအရာများကို ဘယ်လို အသုံးပြုနိုင်မလဲ**: အဖွဲ့များသည် ဤ components များကို အလွယ်တကူ စုပေါင်းပြီး အခြေခံ prototype တစ်ခုကို ဖန်တီးနိုင်သည်။ 

**အကောင်အထည်ဖော်မှုတွင် ဘယ်လို အလုပ်လုပ်သလဲ**: User input မှ အချက်အလက်များကို extract လုပ်ရန် pre-built parser ကို အသုံးပြုခြင်း၊ data ကို သိမ်းဆည်းရန်နှင့် retrieve လုပ်ရန် memory module ကို အသုံးပြုခြင်း၊ user များနှင့် ဆက်သွယ်ရန် prompt generator ကို အသုံးပြုခြင်းတို့ကို လုပ်ဆောင်နိုင်သည်။

**ဥပမာ code**: Semantic Kernel Python နှင့် .Net ကို အသုံးပြု၍ auto-function calling ဖြင့် user input ကို တုံ့ပြန်ပေးသော pre-built AI Connector ကို အသုံးပြုသည့် ဥပမာကို ကြည့်ကြရအောင်:

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

ဤဥပမာတွင် user input မှ origin, destination, date ကဲ့သို့သော အချက်အလက်များကို extract လုပ်ရန် pre-built parser ကို ဘယ်လို အသုံးပြုနိုင်သည်ကို တွေ့ရသည်။ 

### Collaborative Tools ကို အသုံးချခြင်း

CrewAI, Microsoft AutoGen, Semantic Kernel ကဲ့သို့သော frameworks များသည် အခန်းကဏ္ဍများနှင့် အလုပ်များကို သတ်မှတ်ထားသော agent များကို ဖန်တီးရန် အထောက်အကူပေးသည်။

**အဖွဲ့များသည် ဤအရာများကို ဘယ်လို အသုံးပြုနိုင်မလဲ**: အဖွဲ့များသည် agent များကို အခန်းကဏ္ဍများနှင့် အလုပ်များဖြင့် ဒီဇိုင်းဆွဲခြင်း၊ collaborative workflows များကို စမ်းသပ်ခြင်းနှင့် စနစ်၏ ထိရောက်မှုကို တိုးတက်စေရန်။

**အကောင်အထည်ဖော်မှုတွင် ဘယ်လို အလုပ်လုပ်သလဲ**: Data retrieval, analysis, decision-making ကဲ့သို့သော အထူးလုပ်ဆောင်မှုများနှင့် အခန်းကဏ္ဍများရှိသော agent များကို ဖန်တီးနိုင်သည်။ 

**ဥပမာ code (AutoGen)**:

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

ဤ code တွင် agent များသည် data ကို ခွဲခြားလေ့လာရန်အတွက် ပေါင်းစည်းလုပ်ဆောင်မှုကို ပြုလုပ်သည်။

### Real-Time Learning ကို အကောင်အထည်ဖော်ခြင်း

အဆင့်မြင့် frameworks များသည် real-time context ကို နားလည်ခြင်းနှင့် adaptation capabilities များကို ပေးစွမ်းသည်။

**အဖွဲ့များသည် ဤအရာများကို ဘယ်လို အသုံးပြုနိုင်မလဲ**: Feedback loops များကို အကောင်အထည်ဖော်ခြင်း၊ agent များသည် အပြန်အလှန်ဆက်သွယ်မှုများမှ သင်ယူပြီး ၎င်းတို့၏ အပြုအမူကို dynamic အနေဖြင့် ပြင်ဆင်နိုင်သည်။

**အကောင်အထည်ဖော်မှုတွင် ဘယ်လို အလုပ်လုပ်သလဲ**: User feedback, environmental data, task outcomes များကို ခွဲခြားလေ့လာပြီး knowledge base ကို update လုပ်ခြင်း၊ decision-making algorithms ကို ပြင်ဆင်ခြင်းနှင့် စွမ်းဆောင်ရည်ကို တိုးတက်စေခြင်းတို့ကို လုပ်ဆောင်နိုင်သည်။

## AutoGen, Semantic Kernel နှင့် Azure AI Agent Service တို့၏ Frameworks အကြား ကွာခြားချက်များက ဘာလဲ?

Frameworks များကို နှိုင်းယှဉ်ရန် နည်းလမ်းများစွာရှိသော်လည်း ၎င်းတို့၏ ဒီဇိုင်း၊ စွမ်းရည်များနှင့် target use cases အပေါ် အခြေခံ၍ အဓိကကွာခြားချက်များကို ကြည့်ကြရအောင်-

## AutoGen

AutoGen သည် Microsoft Research ရဲ့ AI Frontiers Lab မှ ဖန်တီးထားသော open-source framework ဖြစ်သည်။ ၎င်းသည် event-driven, distributed *agentic* applications ကို အထူးပြုသည်။

AutoGen သည် agent များ၏ core concept အပေါ် အခြေခံထားပြီး agent များသည် ၎င်းတို့၏ ပတ်ဝန်းကျင်ကို သိရှိနိုင်သည်၊ ဆုံးဖြတ်ချက်ချနိုင်သည်၊ သတ်မှတ်ထားသော ရည်မှန်းချက်များကို ရောက်ရှိရန် လုပ်ဆောင်နိုင်သည်။ Agent များသည် asynchronous messages များမှတဆင့် ဆက်သွယ်နိုင်ပြီး parallel အနေဖြင့် အလုပ်လုပ်နိုင်သည်။
## Azure AI Agent Service

Azure AI Agent Service သည် Microsoft Ignite 2024 တွင် မကြာသေးမီက မိတ်ဆက်ခဲ့သော နောက်ဆုံးပေါ်ဝန်ဆောင်မှုတစ်ခုဖြစ်ပြီး၊ Llama 3, Mistral, Cohere စသည့် ဖွင့်လှစ်အရင်းအမြစ် LLM များကို တိုက်ရိုက်ခေါ်ယူနိုင်သည့် ပိုမိုလွယ်ကူသော မော်ဒယ်များဖြင့် AI အေးဂျင့်များကို ဖွံ့ဖြိုးတိုးတက်စေပြီး တပ်ဆင်နိုင်စေသည်။

Azure AI Agent Service သည် လုပ်ငန်းအသုံးချမှုများအတွက် သင့်တော်သော လုံခြုံမှုစနစ်များနှင့် ဒေတာသိုလှောင်မှုနည်းလမ်းများကို ပိုမိုခိုင်မာစေသည်။

ဤဝန်ဆောင်မှုသည် AutoGen နှင့် Semantic Kernel ကဲ့သို့သော မျိုးစုံအေးဂျင့် စီမံခန့်ခွဲမှုဖွဲ့စည်းမှုများနှင့် အလွယ်တကူ ပေါင်းစည်းနိုင်သည်။

လက်ရှိတွင် Public Preview အဆင့်တွင် ရှိပြီး Python နှင့် C# ကို အသုံးပြု၍ အေးဂျင့်များ ဖန်တီးနိုင်သည်။

Semantic Kernel Python ကို အသုံးပြု၍ အသုံးပြုသူက သတ်မှတ်ထားသော plugin ဖြင့် Azure AI Agent တစ်ခု ဖန်တီးနိုင်သည်-

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

### အဓိကအကြောင်းအရာများ

Azure AI Agent Service တွင် အောက်ပါ အဓိကအကြောင်းအရာများ ပါဝင်သည်-

- **Agent**။ Azure AI Agent Service သည် Azure AI Foundry နှင့် ပေါင်းစည်းထားသည်။ AI Foundry အတွင်း AI Agent သည် "စမတ်" မိုက်ခရိုဝန်ဆောင်မှုတစ်ခုအဖြစ် လုပ်ဆောင်ပြီး မေးခွန်းများကို ဖြေကြားခြင်း (RAG), လုပ်ဆောင်မှုများ ပြုလုပ်ခြင်း သို့မဟုတ် လုပ်ငန်းစဉ်များကို အလိုအလျောက်လုပ်ဆောင်ခြင်းတို့ကို ပြုလုပ်နိုင်သည်။ ဤသည်ကို Generative AI မော်ဒယ်များ၏ အင်အားနှင့် အတူ လက်တွေ့ဒေတာရင်းမြစ်များကို အသုံးပြုနိုင်စေသော ကိရိယာများကို ပေါင်းစပ်ခြင်းဖြင့် အောင်မြင်စေသည်။ ဤသည်မှာ အေးဂျင့်တစ်ခု၏ ဥပမာဖြစ်သည်-

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    ဤဥပမာတွင် `gpt-4o-mini` မော်ဒယ်, `my-agent` ဟူသော အမည်နှင့် `You are helpful agent` ဟူသော ညွှန်ကြားချက်များဖြင့် အေးဂျင့်တစ်ခု ဖန်တီးထားသည်။ အေးဂျင့်သည် ကုဒ်အဓိပ္ပါယ်ဖွင့်ဆိုမှု လုပ်ငန်းများကို လုပ်ဆောင်နိုင်ရန် ကိရိယာများနှင့် အရင်းအမြစ်များဖြင့် ပြည့်စုံထားသည်။

- **Thread နှင့် Messages**။ Thread သည် အရေးကြီးသော အခြေခံအကြောင်းအရာတစ်ခုဖြစ်သည်။ ၎င်းသည် အေးဂျင့်နှင့် အသုံးပြုသူအကြား စကားဝိုင်း သို့မဟုတ် အပြန်အလှန်ဆက်သွယ်မှုကို ကိုယ်စားပြုသည်။ Thread များကို စကားဝိုင်း၏ တိုးတက်မှုကို ချုပ်ကိုင်ရန်၊ အကြောင်းအရာအချက်အလက်များကို သိမ်းဆည်းရန်နှင့် အပြန်အလှန်ဆက်သွယ်မှု၏ အခြေအနေကို စီမံခန့်ခွဲရန် အသုံးပြုနိုင်သည်။ ဤသည်မှာ Thread ၏ ဥပမာဖြစ်သည်-

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

    ယခင်ကုဒ်တွင် Thread တစ်ခု ဖန်တီးထားသည်။ ထို့နောက် Thread သို့ Message တစ်ခု ပေးပို့ထားသည်။ `create_and_process_run` ကို ခေါ်ဆိုခြင်းဖြင့် အေးဂျင့်ကို Thread တွင် အလုပ်လုပ်ရန် တိုက်တွန်းထားသည်။ နောက်ဆုံးတွင် Message များကို ရယူပြီး အေးဂျင့်၏ တုံ့ပြန်မှုကို ကြည့်ရှုရန် မှတ်တမ်းတင်ထားသည်။ Message များသည် အသုံးပြုသူနှင့် အေးဂျင့်အကြား စကားဝိုင်း၏ တိုးတက်မှုကို ပြသသည်။ Message များသည် စာသား, ပုံရိပ် သို့မဟုတ် ဖိုင်ကဲ့သို့ အမျိုးအစားအမျိုးမျိုးဖြစ်နိုင်သည်ကိုလည်း နားလည်ရန် အရေးကြီးသည်။ ဥပမာအားဖြင့် အေးဂျင့်၏ အလုပ်သည် ပုံရိပ် သို့မဟုတ် စာသားတုံ့ပြန်မှုတစ်ခုအဖြစ် ရလဒ်ထွက်နိုင်သည်။ Developer အနေဖြင့် ဤအချက်အလက်ကို အသုံးပြု၍ တုံ့ပြန်မှုကို နောက်ထပ်လုပ်ဆောင်ရန် သို့မဟုတ် အသုံးပြုသူထံ တင်ပြရန် အသုံးချနိုင်သည်။

- **အခြား AI ဖွဲ့စည်းမှုများနှင့် ပေါင်းစည်းမှု**။ Azure AI Agent Service သည် AutoGen နှင့် Semantic Kernel ကဲ့သို့သော အခြားဖွဲ့စည်းမှုများနှင့် အပြန်အလှန်ဆက်သွယ်နိုင်သည်။ ၎င်းသည် သင့်အက်ပ်၏ အချို့ကို ဤဖွဲ့စည်းမှုများထဲမှ တစ်ခုတွင် တည်ဆောက်ပြီး၊ ဥပမာအားဖြင့် Agent Service ကို စီမံခန့်ခွဲသူအဖြစ် အသုံးပြုနိုင်သည် သို့မဟုတ် အားလုံးကို Agent Service တွင် တည်ဆောက်နိုင်သည်။

**အသုံးပြုမှုအခွင့်အရေးများ**: Azure AI Agent Service သည် လုံခြုံမှု, အရွယ်အစားနှင့် အလွယ်တကူပြောင်းလွယ်ပြင်လွယ်သော AI အေးဂျင့် တပ်ဆင်မှုများ လိုအပ်သော လုပ်ငန်းအသုံးချမှုများအတွက် ဒီဇိုင်းထုတ်ထားသည်။

## ဤဖွဲ့စည်းမှုများအကြား ကွာခြားချက်များကဘာလဲ?

ဤဖွဲ့စည်းမှုများအကြား အချို့သော ဆင်တူချက်များ ရှိသော်လည်း၊ ၎င်းတို့၏ ဒီဇိုင်း, စွမ်းဆောင်ရည်များနှင့် ရည်ရွယ်ထားသော အသုံးပြုမှုအခွင့်အရေးများတွင် အဓိကကွာခြားချက်များ ရှိသည်-

- **AutoGen**: မျိုးစုံအေးဂျင့်စနစ်များအပေါ် သုတေသနလုပ်ငန်းများအတွက် အထူးသင့်လျော်သော စမ်းသပ်မှုဖွဲ့စည်းမှုဖြစ်သည်။ ရှုပ်ထွေးသော မျိုးစုံအေးဂျင့်စနစ်များကို စမ်းသပ်ရန်နှင့် ပရိုတိုတိုက်ဖျော်ရန် အကောင်းဆုံးနေရာဖြစ်သည်။
- **Semantic Kernel**: လုပ်ငန်းအသုံးချမှုများအတွက် အသင့်ဖြစ်သော အေးဂျင့်စာကြည့်တိုက်ဖြစ်သည်။ အဖြစ်အပျက်အခြေခံ, ဖြန့်ဝေထားသော အေးဂျင့်စနစ်များကို တည်ဆောက်ရန် အထူးပြုသည်။
- **Azure AI Agent Service**: Azure Foundry အတွင်း အေးဂျင့်များအတွက် ပလက်ဖောင်းနှင့် တပ်ဆင်မှုဝန်ဆောင်မှုဖြစ်သည်။ Azure OpenAI, Azure AI Search, Bing Search နှင့် ကုဒ်အကောင်အထည်ဖော်မှုတို့ကို ပေါင်းစည်းမှုများပေးသည်။

မည်သည့်ဖွဲ့စည်းမှုကို ရွေးချယ်ရမည်ဆိုတာ မသေချာဘူးလား?

### အသုံးပြုမှုအခွင့်အရေးများ

အချို့သော ရိုးရိုးရှင်းရှင်း အသုံးပြုမှုအခွင့်အရေးများကို ကြည့်ပြီး သင့်အတွက် အကူအညီပေးကြည့်ရအောင်-

> Q: ငါ စမ်းသပ်နေတယ်၊ သင်ယူနေတယ်၊ အေးဂျင့်အက်ပ်များကို သက်သေပြဖို့ တည်ဆောက်နေတယ်၊ အမြန်တည်ဆောက်ပြီး စမ်းသပ်နိုင်ချင်တယ်။
>
> A: AutoGen သည် ဤအခြေအနေတွင် သင့်တော်သော ရွေးချယ်မှုဖြစ်သည်၊ ၎င်းသည် အဖြစ်အပျက်အခြေခံ, ဖြန့်ဝေထားသော အေးဂျင့်စနစ်များကို အထူးပြုသည်။

> Q: ဤအခွင့်အရေးအတွက် AutoGen သည် Semantic Kernel နှင့် Azure AI Agent Service ထက် ပိုကောင်းသော ရွေးချယ်မှုဖြစ်စေသည့်အရာကဘာလဲ?
>
> A: AutoGen သည် အဖြစ်အပျက်အခြေခံ, ဖြန့်ဝေထားသော အေးဂျင့်စနစ်များအတွက် အထူးဒီဇိုင်းပြုလုပ်ထားပြီး၊ ကုဒ်ထုတ်လုပ်မှုနှင့် ဒေတာခွဲခြမ်းစိတ်ဖြာမှု လုပ်ငန်းများကို အလိုအလျောက်လုပ်ဆောင်ရန် သင့်တော်သည်။

> Q: Azure AI Agent Service သည်လည်း ဤနေရာတွင် အလုပ်လုပ်နိုင်မဟုတ်လား၊ ၎င်းတွင် ကုဒ်ထုတ်လုပ်မှုနှင့် အခြားအရာများအတွက် ကိရိယာများ ရှိတယ်မဟုတ်လား?
>
> A: ဟုတ်ပါတယ်၊ Azure AI Agent Service သည် အေးဂျင့်များအတွက် ပလက်ဖောင်းဝန်ဆောင်မှုဖြစ်ပြီး၊ မော်ဒယ်များစွာ, Azure AI Search, Bing Search နှင့် Azure Functions တို့အတွက် တပ်ဆင်မှုများပါဝင်သည်။

> Q: ကျွန်တော်/ကျွန်မ အခုထိ မသေချာဘူး၊ ရွေးချယ်မှုတစ်ခုပဲ ပြောပြပါ။
>
> A: သင့်အက်ပ်ကို Semantic Kernel တွင် အရင်တည်ဆောက်ပြီး၊ Azure AI Agent Service ကို အသုံးပြု၍ သင့်အေးဂျင့်ကို တပ်ဆင်ပါ။ 

အဓိကကွာခြားချက်များကို ဇယားဖြင့် အကျဉ်းချုပ်ကြည့်ရအောင်-

| ဖွဲ့စည်းမှု | အာရုံစိုက်မှု | အဓိကအကြောင်းအရာများ | အသုံးပြုမှုအခွင့်အရေးများ |
| --- | --- | --- | --- |
| AutoGen | အဖြစ်အပျက်အခြေခံ, ဖြန့်ဝေထားသော အေးဂျင့်စနစ်များ | Agents, Personas, Functions, Data | ကုဒ်ထုတ်လုပ်မှု, ဒေတာခွဲခြမ်းစိတ်ဖြာမှု |
| Semantic Kernel | လူသားဆန်သော စာသားအကြောင်းအရာကို နားလည်ခြင်းနှင့် ထုတ်လုပ်ခြင်း | Agents, Modular Components, Collaboration | သဘာဝဘာသာစကားနားလည်မှု, အကြောင်းအရာထုတ်လုပ်မှု |
| Azure AI Agent Service | Flexible models, လုပ်ငန်းလုံခြုံမှု, ကုဒ်ထုတ်လုပ်မှု, Tool calling | Modularity, Collaboration, Process Orchestration | လုံခြုံမှု, အရွယ်အစားနှင့် ပြောင်းလွယ်ပြင်လွယ်သော AI အေးဂျင့် တပ်ဆင်မှု |

## Azure Ecosystem Tools များကို တိုက်ရိုက်ပေါင်းစည်းနိုင်မလား၊ သီးခြားဖြေရှင်းချက်များလိုအပ်မလား?

အဖြေက ဟုတ်ပါတယ်၊ သင့် Azure Ecosystem Tools များကို Azure AI Agent Service နှင့် တိုက်ရိုက်ပေါင်းစည်းနိုင်သည်။ ဤဝန်ဆောင်မှုသည် Azure ဝန်ဆောင်မှုများနှင့် အလွယ်တကူ ပေါင်းစည်းနိုင်ရန် ဒီဇိုင်းပြုလုပ်ထားသည်။

AutoGen နှင့် Semantic Kernel အတွက်လည်း Azure ဝန်ဆောင်မှုများနှင့် ပေါင်းစည်းနိုင်သော်လည်း၊ သင့်ကုဒ်မှ Azure ဝန်ဆောင်မှုများကို ခေါ်ဆိုရန် လိုအပ်နိုင်သည်။

### AI Agent Frameworks အကြောင်း မေးခွန်းများ ရှိပါသလား?

[Azure AI Foundry Discord](https://aka.ms/ai-agents/discord) တွင် ပါဝင်ပြီး အခြားသင်ယူသူများနှင့် တွေ့ဆုံပါ၊ Office Hours တွင် ပါဝင်ပါ၊ သင့် AI Agents မေးခွန်းများကို ဖြေကြားပါ။

## ကိုးကားချက်များ

- 

## ယခင်သင်ခန်းစာ

[AI Agents နှင့် Agent အသုံးပြုမှုအခွင့်အရေးများကို မိတ်ဆက်ခြင်း](../01-intro-to-ai-agents/README.md)

## နောက်သင်ခန်းစာ

[Agentic Design Patterns ကို နားလည်ခြင်း](../03-agentic-design-patterns/README.md)

---

**ဝက်ဘ်ဆိုက်မှတ်ချက်**:  
ဤစာရွက်စာတမ်းကို AI ဘာသာပြန်ဝန်ဆောင်မှု [Co-op Translator](https://github.com/Azure/co-op-translator) ကို အသုံးပြု၍ ဘာသာပြန်ထားပါသည်။ ကျွန်ုပ်တို့သည် တိကျမှန်ကန်မှုအတွက် ကြိုးစားနေပါသော်လည်း၊ အလိုအလျောက်ဘာသာပြန်မှုများတွင် အမှားများ သို့မဟုတ် မတိကျမှုများ ပါဝင်နိုင်သည်ကို ကျေးဇူးပြု၍ သတိပြုပါ။ မူရင်းစာရွက်စာတမ်းကို ၎င်း၏ မူလဘာသာစကားဖြင့် အာဏာတည်သောရင်းမြစ်အဖြစ် သတ်မှတ်သင့်ပါသည်။ အရေးကြီးသော အချက်အလက်များအတွက် ပရော်ဖက်ရှင်နယ် လူသားဘာသာပြန်မှုကို အကြံပြုပါသည်။ ဤဘာသာပြန်မှုကို အသုံးပြုခြင်းမှ ဖြစ်ပေါ်လာသော နားလည်မှုမှားများ သို့မဟုတ် အဓိပ္ပာယ်မှားများအတွက် ကျွန်ုပ်တို့သည် တာဝန်မယူပါ။