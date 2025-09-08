<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-30T14:04:17+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "hi"
}
-->
[![AI एजेंट फ्रेमवर्क्स का अन्वेषण](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.hi.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(इस पाठ का वीडियो देखने के लिए ऊपर दी गई छवि पर क्लिक करें)_

# AI एजेंट फ्रेमवर्क्स का अन्वेषण

AI एजेंट फ्रेमवर्क्स ऐसे सॉफ़्टवेयर प्लेटफ़ॉर्म हैं जो AI एजेंट्स के निर्माण, परिनियोजन और प्रबंधन को सरल बनाने के लिए डिज़ाइन किए गए हैं। ये फ्रेमवर्क डेवलपर्स को पहले से निर्मित घटकों, अमूर्तताओं और उपकरणों के साथ प्रदान करते हैं, जो जटिल AI सिस्टम के विकास को आसान बनाते हैं।

ये फ्रेमवर्क डेवलपर्स को AI एजेंट विकास में सामान्य चुनौतियों के लिए मानकीकृत दृष्टिकोण प्रदान करके उनके अनुप्रयोगों के अद्वितीय पहलुओं पर ध्यान केंद्रित करने में मदद करते हैं। वे AI सिस्टम के निर्माण में स्केलेबिलिटी, पहुंच और दक्षता को बढ़ाते हैं।

## परिचय

इस पाठ में आप जानेंगे:

- AI एजेंट फ्रेमवर्क्स क्या हैं और वे डेवलपर्स को क्या हासिल करने में सक्षम बनाते हैं?
- टीमें इनका उपयोग करके अपने एजेंट की क्षमताओं को जल्दी से प्रोटोटाइप, पुनरावृत्त और सुधार कैसे कर सकती हैं?
- Microsoft द्वारा बनाए गए फ्रेमवर्क्स और टूल्स में क्या अंतर है?
- क्या मैं अपने मौजूदा Azure इकोसिस्टम टूल्स को सीधे एकीकृत कर सकता हूं, या मुझे स्टैंडअलोन समाधानों की आवश्यकता है?
- Azure AI एजेंट सेवा क्या है और यह मेरी कैसे मदद कर रही है?

## सीखने के लक्ष्य

इस पाठ के लक्ष्य हैं:

- AI विकास में AI एजेंट फ्रेमवर्क्स की भूमिका को समझना।
- AI एजेंट फ्रेमवर्क्स का उपयोग करके बुद्धिमान एजेंट्स का निर्माण करना।
- AI एजेंट फ्रेमवर्क्स द्वारा सक्षम प्रमुख क्षमताओं को समझना।
- AutoGen, Semantic Kernel, और Azure AI एजेंट सेवा के बीच के अंतर को समझना।

## AI एजेंट फ्रेमवर्क्स क्या हैं और वे डेवलपर्स को क्या करने में सक्षम बनाते हैं?

पारंपरिक AI फ्रेमवर्क्स आपके ऐप्स में AI को एकीकृत करने और निम्नलिखित तरीकों से इन ऐप्स को बेहतर बनाने में मदद कर सकते हैं:

- **व्यक्तिकरण (Personalization)**: AI उपयोगकर्ता व्यवहार और प्राथमिकताओं का विश्लेषण करके व्यक्तिगत अनुशंसाएँ, सामग्री और अनुभव प्रदान कर सकता है।  
उदाहरण: Netflix जैसी स्ट्रीमिंग सेवाएं AI का उपयोग करके देखने के इतिहास के आधार पर फिल्में और शो सुझाती हैं, जिससे उपयोगकर्ता की भागीदारी और संतुष्टि बढ़ती है।

- **स्वचालन और दक्षता (Automation and Efficiency)**: AI दोहराए जाने वाले कार्यों को स्वचालित कर सकता है, वर्कफ़्लो को सुव्यवस्थित कर सकता है और परिचालन दक्षता में सुधार कर सकता है।  
उदाहरण: ग्राहक सेवा ऐप्स सामान्य पूछताछ को संभालने के लिए AI-समर्थित चैटबॉट्स का उपयोग करते हैं, प्रतिक्रिया समय को कम करते हैं और जटिल मुद्दों के लिए मानव एजेंटों को मुक्त करते हैं।

- **बेहतर उपयोगकर्ता अनुभव (Enhanced User Experience)**: AI वॉयस रिकग्निशन, नेचुरल लैंग्वेज प्रोसेसिंग और प्रेडिक्टिव टेक्स्ट जैसी बुद्धिमान सुविधाएं प्रदान करके समग्र उपयोगकर्ता अनुभव में सुधार कर सकता है।  
उदाहरण: Siri और Google Assistant जैसे वर्चुअल असिस्टेंट AI का उपयोग करके वॉयस कमांड को समझते और प्रतिक्रिया देते हैं, जिससे उपयोगकर्ताओं के लिए अपने उपकरणों के साथ बातचीत करना आसान हो जाता है।

### यह सब बहुत अच्छा लगता है, तो फिर हमें AI एजेंट फ्रेमवर्क की आवश्यकता क्यों है?

AI एजेंट फ्रेमवर्क्स केवल AI फ्रेमवर्क्स से अधिक का प्रतिनिधित्व करते हैं। इन्हें ऐसे बुद्धिमान एजेंट्स के निर्माण के लिए डिज़ाइन किया गया है जो उपयोगकर्ताओं, अन्य एजेंट्स और पर्यावरण के साथ बातचीत कर सकते हैं और विशिष्ट लक्ष्यों को प्राप्त कर सकते हैं। ये एजेंट्स स्वायत्त व्यवहार प्रदर्शित कर सकते हैं, निर्णय ले सकते हैं और बदलती परिस्थितियों के अनुकूल हो सकते हैं। आइए AI एजेंट फ्रेमवर्क्स द्वारा सक्षम कुछ प्रमुख क्षमताओं पर नज़र डालें:

- **एजेंट सहयोग और समन्वय (Agent Collaboration and Coordination)**: कई AI एजेंट्स के निर्माण को सक्षम बनाना जो एक साथ काम कर सकते हैं, संवाद कर सकते हैं और जटिल कार्यों को हल करने के लिए समन्वय कर सकते हैं।
- **कार्य स्वचालन और प्रबंधन (Task Automation and Management)**: मल्टी-स्टेप वर्कफ़्लो, कार्य प्रतिनिधि और एजेंट्स के बीच गतिशील कार्य प्रबंधन के लिए तंत्र प्रदान करना।
- **प्रासंगिक समझ और अनुकूलन (Contextual Understanding and Adaptation)**: एजेंट्स को संदर्भ को समझने, बदलते परिवेश के अनुकूल होने और वास्तविक समय की जानकारी के आधार पर निर्णय लेने की क्षमता प्रदान करना।

संक्षेप में, एजेंट्स आपको अधिक करने की अनुमति देते हैं, स्वचालन को अगले स्तर तक ले जाते हैं, और अधिक बुद्धिमान सिस्टम बनाने में मदद करते हैं जो अपने पर्यावरण से सीख सकते हैं और अनुकूलित हो सकते हैं।

## एजेंट की क्षमताओं को जल्दी से प्रोटोटाइप, पुनरावृत्त और सुधार कैसे करें?

यह एक तेज़ी से बदलता हुआ क्षेत्र है, लेकिन अधिकांश AI एजेंट फ्रेमवर्क्स में कुछ सामान्य चीजें होती हैं जो आपको जल्दी से प्रोटोटाइप और पुनरावृत्त करने में मदद कर सकती हैं, जैसे मॉड्यूलर घटक, सहयोगी उपकरण, और वास्तविक समय में सीखना। आइए इनमें गहराई से जाएं:

- **मॉड्यूलर घटकों का उपयोग करें (Use Modular Components)**: AI SDKs पहले से निर्मित घटकों जैसे AI और मेमोरी कनेक्टर्स, नेचुरल लैंग्वेज या कोड प्लगइन्स का उपयोग करके फ़ंक्शन कॉलिंग, प्रॉम्प्ट टेम्पलेट्स आदि प्रदान करते हैं।
- **सहयोगी उपकरणों का लाभ उठाएं (Leverage Collaborative Tools)**: विशिष्ट भूमिकाओं और कार्यों के साथ एजेंट्स को डिज़ाइन करें, जिससे सहयोगी वर्कफ़्लो का परीक्षण और परिष्कृत किया जा सके।
- **वास्तविक समय में सीखें (Learn in Real-Time)**: फीडबैक लूप्स को लागू करें जहां एजेंट्स इंटरैक्शन से सीखते हैं और अपने व्यवहार को गतिशील रूप से समायोजित करते हैं।

### मॉड्यूलर घटकों का उपयोग करें

Microsoft Semantic Kernel और LangChain जैसे SDKs पहले से निर्मित घटकों जैसे AI कनेक्टर्स, प्रॉम्प्ट टेम्पलेट्स और मेमोरी प्रबंधन की पेशकश करते हैं।

**टीमें इनका उपयोग कैसे कर सकती हैं**: टीमें इन घटकों को जल्दी से इकट्ठा करके एक कार्यात्मक प्रोटोटाइप बना सकती हैं, जिससे बिना शुरुआत से शुरू किए तेजी से प्रयोग और पुनरावृत्ति की जा सके।

**यह व्यावहारिक रूप से कैसे काम करता है**: आप उपयोगकर्ता इनपुट से जानकारी निकालने के लिए एक पहले से निर्मित पार्सर, डेटा को संग्रहीत और पुनः प्राप्त करने के लिए एक मेमोरी मॉड्यूल, और उपयोगकर्ताओं के साथ बातचीत करने के लिए एक प्रॉम्प्ट जेनरेटर का उपयोग कर सकते हैं, वह भी बिना इन घटकों को खरोंच से बनाए।

**उदाहरण कोड**। आइए देखें कि आप Semantic Kernel Python और .Net के साथ एक पहले से निर्मित AI कनेक्टर का उपयोग कैसे कर सकते हैं जो उपयोगकर्ता इनपुट का जवाब देने के लिए ऑटो-फ़ंक्शन कॉलिंग का उपयोग करता है:

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

इस उदाहरण से आप देख सकते हैं कि आप उपयोगकर्ता इनपुट से मूलभूत जानकारी जैसे उड़ान बुकिंग अनुरोध की उत्पत्ति, गंतव्य और तारीख निकालने के लिए एक पहले से निर्मित पार्सर का उपयोग कैसे कर सकते हैं। यह मॉड्यूलर दृष्टिकोण आपको उच्च-स्तरीय तर्क पर ध्यान केंद्रित करने की अनुमति देता है।

### सहयोगी उपकरणों का लाभ उठाएं

CrewAI, Microsoft AutoGen, और Semantic Kernel जैसे फ्रेमवर्क कई एजेंट्स के निर्माण को सुविधाजनक बनाते हैं जो एक साथ काम कर सकते हैं।

**टीमें इनका उपयोग कैसे कर सकती हैं**: टीमें विशिष्ट भूमिकाओं और कार्यों के साथ एजेंट्स को डिज़ाइन कर सकती हैं, जिससे सहयोगी वर्कफ़्लो का परीक्षण और परिष्कृत किया जा सके और समग्र सिस्टम दक्षता में सुधार किया जा सके।

**यह व्यावहारिक रूप से कैसे काम करता है**: आप एजेंट्स की एक टीम बना सकते हैं जहां प्रत्येक एजेंट का एक विशेष कार्य होता है, जैसे डेटा पुनर्प्राप्ति, विश्लेषण, या निर्णय लेना। ये एजेंट्स एक सामान्य लक्ष्य प्राप्त करने के लिए संवाद कर सकते हैं और जानकारी साझा कर सकते हैं, जैसे उपयोगकर्ता की क्वेरी का उत्तर देना या कोई कार्य पूरा करना।

**उदाहरण कोड (AutoGen)**:

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

पिछले कोड में, आप देख सकते हैं कि कैसे आप एक ऐसा कार्य बना सकते हैं जिसमें कई एजेंट्स डेटा का विश्लेषण करने के लिए एक साथ काम करते हैं। प्रत्येक एजेंट एक विशिष्ट कार्य करता है, और कार्य को वांछित परिणाम प्राप्त करने के लिए एजेंट्स को समन्वित करके निष्पादित किया जाता है। विशेष भूमिकाओं वाले समर्पित एजेंट्स बनाकर, आप कार्य की दक्षता और प्रदर्शन में सुधार कर सकते हैं।

### वास्तविक समय में सीखें

उन्नत फ्रेमवर्क वास्तविक समय में संदर्भ को समझने और अनुकूलन करने की क्षमताएं प्रदान करते हैं।

**टीमें इनका उपयोग कैसे कर सकती हैं**: टीमें फीडबैक लूप्स को लागू कर सकती हैं जहां एजेंट्स इंटरैक्शन से सीखते हैं और अपने व्यवहार को गतिशील रूप से समायोजित करते हैं, जिससे क्षमताओं में निरंतर सुधार और परिष्करण होता है।

**यह व्यावहारिक रूप से कैसे काम करता है**: एजेंट्स उपयोगकर्ता फीडबैक, पर्यावरणीय डेटा, और कार्य परिणामों का विश्लेषण कर सकते हैं ताकि अपने ज्ञान आधार को अपडेट कर सकें, निर्णय लेने के एल्गोरिदम को समायोजित कर सकें, और समय के साथ प्रदर्शन में सुधार कर सकें। यह पुनरावृत्त सीखने की प्रक्रिया एजेंट्स को बदलती परिस्थितियों और उपयोगकर्ता प्राथमिकताओं के अनुकूल होने में सक्षम बनाती है, जिससे समग्र सिस्टम प्रभावशीलता बढ़ती है।

## AutoGen, Semantic Kernel और Azure AI एजेंट सेवा के बीच क्या अंतर है?

इन फ्रेमवर्क्स की तुलना करने के कई तरीके हैं, लेकिन आइए उनके डिज़ाइन, क्षमताओं और लक्षित उपयोग मामलों के संदर्भ में कुछ प्रमुख अंतरों पर नज़र डालें:

## AutoGen

AutoGen Microsoft Research के AI Frontiers Lab द्वारा विकसित एक ओपन-सोर्स फ्रेमवर्क है। यह इवेंट-ड्रिवन, वितरित *एजेंटिक* अनुप्रयोगों पर केंद्रित है, जो कई LLMs और SLMs, टूल्स, और उन्नत मल्टी-एजेंट डिज़ाइन पैटर्न को सक्षम बनाता है।

AutoGen एजेंट्स के मुख्य विचार के इर्द-गिर्द निर्मित है, जो स्वायत्त संस्थाएं हैं जो अपने पर्यावरण को समझ सकती हैं, निर्णय ले सकती हैं, और विशिष्ट लक्ष्यों को प्राप्त करने के लिए कार्य कर सकती हैं। एजेंट्स एसिंक्रोनस संदेशों के माध्यम से संवाद करते हैं, जिससे वे स्वतंत्र रूप से और समानांतर में काम कर सकते हैं, सिस्टम की स्केलेबिलिटी और उत्तरदायित्व को बढ़ा सकते हैं।
तो यह था Semantic Kernel फ्रेमवर्क का मूल परिचय, अब बात करते हैं Agent Framework की।

## Azure AI Agent Service

Azure AI Agent Service एक नया फीचर है, जिसे Microsoft Ignite 2024 में पेश किया गया। यह AI एजेंट्स को अधिक लचीले मॉडल्स के साथ विकसित और तैनात करने की अनुमति देता है, जैसे कि सीधे ओपन-सोर्स LLMs जैसे Llama 3, Mistral, और Cohere को कॉल करना।

Azure AI Agent Service मजबूत एंटरप्राइज़ सुरक्षा तंत्र और डेटा स्टोरेज विधियों को प्रदान करता है, जिससे यह एंटरप्राइज़ एप्लिकेशन के लिए उपयुक्त बनता है।

यह AutoGen और Semantic Kernel जैसे मल्टी-एजेंट ऑर्केस्ट्रेशन फ्रेमवर्क्स के साथ आसानी से काम करता है।

यह सेवा वर्तमान में Public Preview में है और Python और C# को एजेंट्स बनाने के लिए सपोर्ट करती है।

Semantic Kernel Python का उपयोग करके, हम एक यूजर-डिफाइंड प्लगइन के साथ Azure AI Agent बना सकते हैं:

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

### मुख्य अवधारणाएँ

Azure AI Agent Service में निम्नलिखित मुख्य अवधारणाएँ हैं:

- **Agent**: Azure AI Agent Service, Azure AI Foundry के साथ इंटीग्रेट करता है। AI Foundry के भीतर, एक AI Agent एक "स्मार्ट" माइक्रोसर्विस के रूप में कार्य करता है, जिसका उपयोग सवालों का जवाब देने (RAG), कार्य करने, या वर्कफ्लो को पूरी तरह से ऑटोमेट करने के लिए किया जा सकता है। यह जनरेटिव AI मॉडल्स की शक्ति को वास्तविक दुनिया के डेटा स्रोतों तक पहुंचने और उनके साथ इंटरैक्ट करने वाले टूल्स के साथ जोड़कर इसे प्राप्त करता है। यहाँ एक एजेंट का उदाहरण है:

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    इस उदाहरण में, एक एजेंट `gpt-4o-mini` मॉडल, नाम `my-agent`, और निर्देश `You are helpful agent` के साथ बनाया गया है। एजेंट को कोड इंटरप्रिटेशन कार्यों को करने के लिए टूल्स और संसाधनों से लैस किया गया है।

- **Thread और Messages**: थ्रेड एक और महत्वपूर्ण अवधारणा है। यह एक एजेंट और उपयोगकर्ता के बीच बातचीत या इंटरैक्शन को दर्शाता है। थ्रेड्स का उपयोग बातचीत की प्रगति को ट्रैक करने, संदर्भ जानकारी को स्टोर करने, और इंटरैक्शन की स्थिति को प्रबंधित करने के लिए किया जा सकता है। यहाँ एक थ्रेड का उदाहरण है:

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

    पिछले कोड में, एक थ्रेड बनाया गया है। इसके बाद, थ्रेड को एक संदेश भेजा गया है। `create_and_process_run` को कॉल करके, एजेंट को थ्रेड पर काम करने के लिए कहा गया है। अंत में, संदेशों को प्राप्त और लॉग किया गया है ताकि एजेंट की प्रतिक्रिया देखी जा सके। संदेश उपयोगकर्ता और एजेंट के बीच बातचीत की प्रगति को दर्शाते हैं। यह भी महत्वपूर्ण है कि संदेश विभिन्न प्रकार के हो सकते हैं जैसे टेक्स्ट, इमेज, या फाइल, जो एजेंट के काम का परिणाम हो सकता है। उदाहरण के लिए, एक इमेज या टेक्स्ट प्रतिक्रिया। एक डेवलपर के रूप में, आप इस जानकारी का उपयोग प्रतिक्रिया को आगे प्रोसेस करने या उपयोगकर्ता को प्रस्तुत करने के लिए कर सकते हैं।

- **अन्य AI फ्रेमवर्क्स के साथ इंटीग्रेशन**: Azure AI Agent Service अन्य फ्रेमवर्क्स जैसे AutoGen और Semantic Kernel के साथ इंटरैक्ट कर सकता है, जिसका मतलब है कि आप अपने ऐप का एक हिस्सा इनमें से किसी एक फ्रेमवर्क में बना सकते हैं और उदाहरण के लिए Agent Service का उपयोग ऑर्केस्ट्रेटर के रूप में कर सकते हैं या आप सब कुछ Agent Service में बना सकते हैं।

**Use Cases**: Azure AI Agent Service को एंटरप्राइज़ एप्लिकेशन के लिए डिज़ाइन किया गया है, जिन्हें सुरक्षित, स्केलेबल, और लचीले AI एजेंट डिप्लॉयमेंट की आवश्यकता होती है।

## इन फ्रेमवर्क्स में क्या अंतर है?

ऐसा लगता है कि इन फ्रेमवर्क्स में काफी ओवरलैप है, लेकिन उनके डिज़ाइन, क्षमताओं, और लक्षित उपयोग मामलों के संदर्भ में कुछ प्रमुख अंतर हैं:

- **AutoGen**: यह मल्टी-एजेंट सिस्टम्स पर अग्रणी शोध के लिए एक प्रयोगात्मक फ्रेमवर्क है। यह जटिल मल्टी-एजेंट सिस्टम्स को प्रोटोटाइप और एक्सपेरिमेंट करने के लिए सबसे अच्छा स्थान है।
- **Semantic Kernel**: यह एंटरप्राइज़ एजेंटिक एप्लिकेशन बनाने के लिए एक प्रोडक्शन-रेडी एजेंट लाइब्रेरी है। यह इवेंट-ड्रिवन, डिस्ट्रीब्यूटेड एजेंटिक एप्लिकेशन पर केंद्रित है, जो कई LLMs और SLMs, टूल्स, और सिंगल/मल्टी-एजेंट डिज़ाइन पैटर्न को सक्षम बनाता है।
- **Azure AI Agent Service**: यह Azure Foundry में एजेंट्स के लिए एक प्लेटफ़ॉर्म और डिप्लॉयमेंट सेवा है। यह Azure OpenAI, Azure AI Search, Bing Search और कोड एक्सेक्यूशन जैसे सेवाओं के साथ कनेक्टिविटी प्रदान करता है।

अब भी तय नहीं कर पा रहे कि कौन सा चुनें?

### उपयोग के मामले

आइए कुछ सामान्य उपयोग मामलों के माध्यम से आपकी मदद करने की कोशिश करते हैं:

> Q: मैं प्रयोग कर रहा हूँ, सीख रहा हूँ और प्रूफ-ऑफ-कॉन्सेप्ट एजेंट एप्लिकेशन बना रहा हूँ, और मैं जल्दी से निर्माण और प्रयोग करना चाहता हूँ।

> A: AutoGen इस स्थिति के लिए एक अच्छा विकल्प होगा, क्योंकि यह इवेंट-ड्रिवन, डिस्ट्रीब्यूटेड एजेंटिक एप्लिकेशन पर केंद्रित है और उन्नत मल्टी-एजेंट डिज़ाइन पैटर्न को सपोर्ट करता है।

> Q: इस उपयोग मामले के लिए Semantic Kernel और Azure AI Agent Service की तुलना में AutoGen को बेहतर विकल्प क्यों माना जाता है?

> A: AutoGen विशेष रूप से इवेंट-ड्रिवन, डिस्ट्रीब्यूटेड एजेंटिक एप्लिकेशन के लिए डिज़ाइन किया गया है, जो कोड जनरेशन और डेटा एनालिसिस कार्यों को ऑटोमेट करने के लिए उपयुक्त है। यह जटिल मल्टी-एजेंट सिस्टम्स को कुशलतापूर्वक बनाने के लिए आवश्यक टूल्स और क्षमताएँ प्रदान करता है।

> Q: लगता है Azure AI Agent Service भी यहाँ काम कर सकता है, इसमें कोड जनरेशन और अन्य टूल्स हैं?

> A: हाँ, Azure AI Agent Service एजेंट्स के लिए एक प्लेटफ़ॉर्म सेवा है और इसमें कई मॉडल्स, Azure AI Search, Bing Search और Azure Functions के लिए बिल्ट-इन क्षमताएँ हैं। यह Foundry Portal में आपके एजेंट्स को बनाना और उन्हें बड़े पैमाने पर तैनात करना आसान बनाता है।

> Q: मैं अब भी उलझन में हूँ, बस एक विकल्प बता दीजिए।

> A: एक अच्छा विकल्प है कि आप पहले Semantic Kernel में अपना एप्लिकेशन बनाएं और फिर Azure AI Agent Service का उपयोग करके अपने एजेंट को तैनात करें। यह दृष्टिकोण आपको अपने एजेंट्स को आसानी से बनाए रखने की अनुमति देता है, साथ ही Semantic Kernel में मल्टी-एजेंट सिस्टम्स बनाने की शक्ति का लाभ उठाने देता है। इसके अलावा, Semantic Kernel में AutoGen के लिए एक कनेक्टर है, जिससे दोनों फ्रेमवर्क्स को एक साथ उपयोग करना आसान हो जाता है।

आइए इन फ्रेमवर्क्स के प्रमुख अंतर को एक तालिका में संक्षेप करें:

| फ्रेमवर्क | फोकस | मुख्य अवधारणाएँ | उपयोग के मामले |
| --- | --- | --- | --- |
| AutoGen | इवेंट-ड्रिवन, डिस्ट्रीब्यूटेड एजेंटिक एप्लिकेशन | एजेंट्स, पर्सनाज, फंक्शन्स, डेटा | कोड जनरेशन, डेटा एनालिसिस कार्य |
| Semantic Kernel | मानव-जैसे टेक्स्ट कंटेंट को समझना और जनरेट करना | एजेंट्स, मॉड्यूलर कंपोनेंट्स, सहयोग | प्राकृतिक भाषा समझना, कंटेंट जनरेशन |
| Azure AI Agent Service | लचीले मॉडल्स, एंटरप्राइज़ सुरक्षा, कोड जनरेशन, टूल कॉलिंग | मॉड्यूलरिटी, सहयोग, प्रक्रिया ऑर्केस्ट्रेशन | सुरक्षित, स्केलेबल, और लचीले AI एजेंट डिप्लॉयमेंट |

इन फ्रेमवर्क्स के लिए आदर्श उपयोग मामला क्या है?

## क्या मैं अपने मौजूदा Azure इकोसिस्टम टूल्स को सीधे इंटीग्रेट कर सकता हूँ, या मुझे स्टैंडअलोन सॉल्यूशन्स की आवश्यकता है?

उत्तर है हाँ, आप अपने मौजूदा Azure इकोसिस्टम टूल्स को सीधे Azure AI Agent Service के साथ इंटीग्रेट कर सकते हैं, खासकर क्योंकि इसे अन्य Azure सेवाओं के साथ सहजता से काम करने के लिए बनाया गया है। उदाहरण के लिए, आप Bing, Azure AI Search, और Azure Functions को इंटीग्रेट कर सकते हैं। Azure AI Foundry के साथ भी गहरा इंटीग्रेशन है।

AutoGen और Semantic Kernel के लिए, आप Azure सेवाओं के साथ भी इंटीग्रेट कर सकते हैं, लेकिन इसके लिए आपको अपने कोड से Azure सेवाओं को कॉल करना पड़ सकता है। एक और तरीका है Azure SDKs का उपयोग करके अपने एजेंट्स से Azure सेवाओं के साथ इंटरैक्ट करना। इसके अलावा, जैसा कि पहले बताया गया, आप AutoGen या Semantic Kernel में बनाए गए एजेंट्स के लिए Azure AI Agent Service को ऑर्केस्ट्रेटर के रूप में उपयोग कर सकते हैं, जिससे Azure इकोसिस्टम तक आसान पहुंच मिलती है।

### AI Agent Frameworks के बारे में और सवाल हैं?

[Azure AI Foundry Discord](https://aka.ms/ai-agents/discord) से जुड़ें, अन्य शिक्षार्थियों से मिलें, ऑफिस आवर्स में भाग लें और अपने AI Agents से जुड़े सवालों के जवाब पाएं।

## संदर्भ

- 

## पिछला पाठ

[AI Agents और उनके उपयोग मामलों का परिचय](../01-intro-to-ai-agents/README.md)

## अगला पाठ

[Agentic डिज़ाइन पैटर्न को समझना](../03-agentic-design-patterns/README.md)

---

**अस्वीकरण**:  
यह दस्तावेज़ AI अनुवाद सेवा [Co-op Translator](https://github.com/Azure/co-op-translator) का उपयोग करके अनुवादित किया गया है। जबकि हम सटीकता सुनिश्चित करने का प्रयास करते हैं, कृपया ध्यान दें कि स्वचालित अनुवाद में त्रुटियां या अशुद्धियां हो सकती हैं। मूल भाषा में उपलब्ध मूल दस्तावेज़ को प्रामाणिक स्रोत माना जाना चाहिए। महत्वपूर्ण जानकारी के लिए, पेशेवर मानव अनुवाद की सिफारिश की जाती है। इस अनुवाद के उपयोग से उत्पन्न किसी भी गलतफहमी या गलत व्याख्या के लिए हम जिम्मेदार नहीं हैं।