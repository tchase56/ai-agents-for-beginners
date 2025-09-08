<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-29T10:21:39+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "ne"
}
-->
[![AI एजेन्ट फ्रेमवर्क्स अन्वेषण गर्दै](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.ne.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(यो पाठको भिडियो हेर्न माथिको तस्बिरमा क्लिक गर्नुहोस्)_

# एआई एजेन्ट फ्रेमवर्क्स अन्वेषण गर्नुहोस्

एआई एजेन्ट फ्रेमवर्कहरू एआई एजेन्टहरू सिर्जना, परिनियोजन, र व्यवस्थापन गर्न सजिलो बनाउने सफ्टवेयर प्लेटफर्महरू हुन्। यी फ्रेमवर्कहरूले विकासकर्ताहरूलाई पूर्व-निर्मित कम्पोनेन्टहरू, अमूर्तताहरू, र उपकरणहरू प्रदान गर्छन् जसले जटिल एआई प्रणालीहरूको विकासलाई सरल बनाउँछ।

यी फ्रेमवर्कहरूले एआई एजेन्ट विकासमा सामान्य चुनौतीहरूको लागि मानकीकृत दृष्टिकोण प्रदान गरेर विकासकर्ताहरूलाई उनीहरूको अनुप्रयोगहरूको अद्वितीय पक्षहरूमा ध्यान केन्द्रित गर्न मद्दत गर्छन्। तिनीहरूले एआई प्रणालीहरू निर्माण गर्दा मापनयोग्यता, पहुँचयोग्यता, र दक्षता बढाउँछन्।

## परिचय

यो पाठले समेट्नेछ:

- एआई एजेन्ट फ्रेमवर्कहरू के हुन् र तिनीहरूले विकासकर्ताहरूलाई के हासिल गर्न सक्षम बनाउँछन्?
- टोलीहरूले कसरी यी फ्रेमवर्कहरू प्रयोग गरेर छिटो प्रोटोटाइप बनाउन, दोहोर्याउन, र एजेन्टको क्षमताहरू सुधार गर्न सक्छन्?
- माइक्रोसफ्टद्वारा सिर्जना गरिएका फ्रेमवर्कहरू र उपकरणहरू बीच के फरक छ?
- के म मेरो विद्यमान Azure इकोसिस्टम उपकरणहरू सिधै एकीकृत गर्न सक्छु, वा मलाई छुट्टै समाधानहरू चाहिन्छ?
- Azure AI Agents सेवा के हो र यसले मलाई कसरी मद्दत गरिरहेको छ?

## सिकाइका लक्ष्यहरू

यो पाठको लक्ष्य तपाईंलाई निम्न कुरा बुझ्न मद्दत गर्नु हो:

- एआई विकासमा एआई एजेन्ट फ्रेमवर्कहरूको भूमिका।
- एआई एजेन्ट फ्रेमवर्कहरूको उपयोग गरेर बौद्धिक एजेन्टहरू कसरी निर्माण गर्ने।
- एआई एजेन्ट फ्रेमवर्कहरूले सक्षम बनाउने प्रमुख क्षमताहरू।
- AutoGen, Semantic Kernel, र Azure AI Agent Service बीचका भिन्नताहरू।

## एआई एजेन्ट फ्रेमवर्कहरू के हुन् र तिनीहरूले विकासकर्ताहरूलाई के गर्न सक्षम बनाउँछन्?

परम्परागत एआई फ्रेमवर्कहरूले तपाईंलाई एआईलाई तपाईंको अनुप्रयोगहरूमा एकीकृत गर्न र निम्न तरिकामा यी अनुप्रयोगहरूलाई सुधार गर्न मद्दत गर्न सक्छ:

- **व्यक्तिगतकरण**: एआईले प्रयोगकर्ताको व्यवहार र प्राथमिकताहरू विश्लेषण गरेर व्यक्तिगत सिफारिसहरू, सामग्री, र अनुभवहरू प्रदान गर्न सक्छ।
उदाहरण: Netflix जस्ता स्ट्रिमिङ सेवाहरूले एआई प्रयोग गरेर हेर्ने इतिहासको आधारमा चलचित्र र शोहरू सुझाव दिन्छन्, जसले प्रयोगकर्ताको संलग्नता र सन्तुष्टि बढाउँछ।
- **स्वचालन र दक्षता**: एआईले दोहोरिने कार्यहरू स्वचालित गर्न, कार्यप्रवाहहरू सरल बनाउन, र सञ्चालन दक्षता सुधार गर्न सक्छ।
उदाहरण: ग्राहक सेवा अनुप्रयोगहरूले सामान्य सोधपुछहरूलाई सम्बोधन गर्न एआई-संचालित च्याटबोटहरू प्रयोग गर्छन्, प्रतिक्रिया समय घटाउँछन् र जटिल मुद्दाहरूका लागि मानव एजेन्टहरूलाई स्वतन्त्र बनाउँछन्।
- **प्रयोगकर्ता अनुभव सुधार**: एआईले आवाज पहिचान, प्राकृतिक भाषा प्रशोधन, र भविष्यवाणी पाठ जस्ता बौद्धिक सुविधाहरू प्रदान गरेर समग्र प्रयोगकर्ता अनुभव सुधार गर्न सक्छ।
उदाहरण: Siri र Google Assistant जस्ता भर्चुअल सहायकहरूले एआई प्रयोग गरेर आवाज आदेशहरू बुझ्छन् र प्रतिक्रिया दिन्छन्, जसले प्रयोगकर्ताहरूलाई उनीहरूको उपकरणहरूसँग अन्तरक्रिया गर्न सजिलो बनाउँछ।

### यो सबै राम्रो सुनिन्छ, हैन? त्यसो भए हामीलाई एआई एजेन्ट फ्रेमवर्क किन चाहिन्छ?

एआई एजेन्ट फ्रेमवर्कहरू केवल एआई फ्रेमवर्कहरू भन्दा बढी प्रतिनिधित्व गर्छन्। तिनीहरू बौद्धिक एजेन्टहरू सिर्जना गर्न डिजाइन गरिएका छन् जसले प्रयोगकर्ताहरू, अन्य एजेन्टहरू, र वातावरणसँग अन्तरक्रिया गर्न सक्छन् ताकि विशिष्ट लक्ष्यहरू प्राप्त गर्न सकियोस्। यी एजेन्टहरूले स्वायत्त व्यवहार प्रदर्शन गर्न सक्छन्, निर्णय लिन सक्छन्, र परिवर्तनशील अवस्थाहरूमा अनुकूलन गर्न सक्छन्। एआई एजेन्ट फ्रेमवर्कहरूले सक्षम बनाउने केही प्रमुख क्षमताहरू हेरौं:

- **एजेन्ट सहयोग र समन्वय**: धेरै एआई एजेन्टहरू सिर्जना गर्न सक्षम बनाउनुहोस् जसले सँगै काम गर्न, संवाद गर्न, र जटिल कार्यहरू समाधान गर्न समन्वय गर्न सक्छन्।
- **कार्य स्वचालन र व्यवस्थापन**: बहु-चरण कार्यप्रवाहहरू स्वचालित गर्न, कार्य प्रतिनिधित्व गर्न, र एजेन्टहरू बीच गतिशील कार्य व्यवस्थापनका लागि संयन्त्रहरू प्रदान गर्नुहोस्।
- **सन्दर्भीय समझ र अनुकूलन**: एजेन्टहरूलाई सन्दर्भ बुझ्न, परिवर्तनशील वातावरणमा अनुकूलन गर्न, र वास्तविक-समय जानकारीको आधारमा निर्णय लिन सक्षम बनाउनुहोस्।

सारांशमा, एजेन्टहरूले तपाईंलाई अझ धेरै गर्न, स्वचालनलाई अर्को स्तरमा लैजान, र वातावरणबाट सिक्न र अनुकूलन गर्न सक्षम थप बौद्धिक प्रणालीहरू सिर्जना गर्न अनुमति दिन्छन्।

## कसरी छिटो प्रोटोटाइप बनाउन, दोहोर्याउन, र एजेन्टको क्षमताहरू सुधार गर्ने?

यो छिटो परिवर्तन हुने क्षेत्र हो, तर त्यहाँ केही चीजहरू छन् जुन अधिकांश एआई एजेन्ट फ्रेमवर्कहरूमा सामान्य छन् जसले तपाईंलाई छिटो प्रोटोटाइप बनाउन र दोहोर्याउन मद्दत गर्न सक्छ, जस्तै मोड्युलर कम्पोनेन्टहरू, सहयोगात्मक उपकरणहरू, र वास्तविक-समय सिकाइ। यी विषयहरूमा गहिराइमा जाऔं:

- **मोड्युलर कम्पोनेन्टहरू प्रयोग गर्नुहोस्**: एआई SDKहरूले पूर्व-निर्मित कम्पोनेन्टहरू प्रदान गर्छन् जस्तै एआई र मेमोरी कनेक्टरहरू, प्राकृतिक भाषाको प्रयोग गरेर कार्य कलिंग, प्रम्प्ट टेम्प्लेटहरू, र थप।
- **सहयोगात्मक उपकरणहरूको लाभ उठाउनुहोस्**: विशिष्ट भूमिकाहरू र कार्यहरूसहित एजेन्टहरू डिजाइन गर्नुहोस्, जसले सहयोगात्मक कार्यप्रवाहहरू परीक्षण र परिष्कृत गर्न सक्षम बनाउँछ।
- **वास्तविक-समयमा सिक्नुहोस्**: प्रतिक्रिया लूपहरू कार्यान्वयन गर्नुहोस् जहाँ एजेन्टहरूले अन्तरक्रियाबाट सिक्छन् र गतिशील रूपमा आफ्नो व्यवहार समायोजन गर्छन्।

### मोड्युलर कम्पोनेन्टहरू प्रयोग गर्नुहोस्

Microsoft Semantic Kernel र LangChain जस्ता SDKहरूले पूर्व-निर्मित कम्पोनेन्टहरू प्रदान गर्छन् जस्तै एआई कनेक्टरहरू, प्रम्प्ट टेम्प्लेटहरू, र मेमोरी व्यवस्थापन।

**टोलीहरूले यसलाई कसरी प्रयोग गर्न सक्छन्**: टोलीहरूले यी कम्पोनेन्टहरूलाई छिटो कार्यात्मक प्रोटोटाइप बनाउनका लागि जम्मा गर्न सक्छन्, जसले सुरुबाट सुरु नगरी छिटो प्रयोग र दोहोर्याउन अनुमति दिन्छ।

**यसले व्यवहारमा कसरी काम गर्छ**: तपाईंले प्रयोगकर्ताको इनपुटबाट जानकारी निकाल्न पूर्व-निर्मित पार्सर, डेटा भण्डारण र पुनःप्राप्त गर्न मेमोरी मोड्युल, र प्रयोगकर्ताहरूसँग अन्तरक्रिया गर्न प्रम्प्ट जेनेरेटर प्रयोग गर्न सक्नुहुन्छ, यी कम्पोनेन्टहरू सुरुबाट निर्माण नगरी।

**उदाहरण कोड**। Semantic Kernel Python र .Net प्रयोग गरेर पूर्व-निर्मित एआई कनेक्टरको प्रयोग गरेर प्रयोगकर्ताको इनपुटमा प्रतिक्रिया दिन मोडेलले कसरी स्वत: कार्य कलिंग प्रयोग गर्न सक्छ भन्ने उदाहरणहरू हेरौं:

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

यस उदाहरणबाट तपाईंले देख्न सक्नुहुन्छ कि कसरी पूर्व-निर्मित पार्सर प्रयोग गरेर प्रयोगकर्ताको इनपुटबाट प्रमुख जानकारीहरू निकाल्न सकिन्छ, जस्तै उडान बुकिङ अनुरोधको उत्पत्ति, गन्तव्य, र मिति। यो मोड्युलर दृष्टिकोणले तपाईंलाई उच्च-स्तरीय तर्कमा ध्यान केन्द्रित गर्न अनुमति दिन्छ।

### सहयोगात्मक उपकरणहरूको लाभ उठाउनुहोस्

CrewAI, Microsoft AutoGen, र Semantic Kernel जस्ता फ्रेमवर्कहरूले सँगै काम गर्न सक्ने धेरै एजेन्टहरूको सिर्जना गर्न सुविधा दिन्छन्।

**टोलीहरूले यसलाई कसरी प्रयोग गर्न सक्छन्**: टोलीहरूले विशिष्ट कार्यहरू र भूमिकाहरूका साथ एजेन्टहरू डिजाइन गर्न सक्छन्, जसले सहयोगात्मक कार्यप्रवाहहरू परीक्षण र परिष्कृत गर्न र समग्र प्रणाली दक्षता सुधार गर्न सक्षम बनाउँछ।

**यसले व्यवहारमा कसरी काम गर्छ**: तपाईंले डेटा पुनःप्राप्ति, विश्लेषण, वा निर्णय-निर्माण जस्ता विशेष कार्यहरू भएका एजेन्टहरूको टोली सिर्जना गर्न सक्नुहुन्छ। यी एजेन्टहरूले जानकारी साझा गर्न र साझा लक्ष्य प्राप्त गर्न, जस्तै प्रयोगकर्ताको सोधपुछको उत्तर दिन वा कार्य पूरा गर्न संवाद गर्न सक्छन्।

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

अघिल्लो कोडमा तपाईंले देख्न सक्नुहुन्छ कि कसरी डेटा विश्लेषण गर्न धेरै एजेन्टहरू समावेश गर्ने कार्य सिर्जना गर्न सकिन्छ। प्रत्येक एजेन्टले विशिष्ट कार्य गर्दछ, र कार्यलाई समन्वय गरेर इच्छित परिणाम प्राप्त गर्न एजेन्टहरूको समन्वय गरेर कार्यान्वयन गरिन्छ। विशेष भूमिकाहरू भएका समर्पित एजेन्टहरू सिर्जना गरेर, तपाईं कार्य दक्षता र प्रदर्शन सुधार गर्न सक्नुहुन्छ।

### वास्तविक-समयमा सिक्नुहोस्

उन्नत फ्रेमवर्कहरूले वास्तविक-समय सन्दर्भ समझ र अनुकूलनका लागि क्षमताहरू प्रदान गर्छन्।

**टोलीहरूले यसलाई कसरी प्रयोग गर्न सक्छन्**: टोलीहरूले प्रतिक्रिया लूपहरू कार्यान्वयन गर्न सक्छन् जहाँ एजेन्टहरूले अन्तरक्रियाबाट सिक्छन् र गतिशील रूपमा आफ्नो व्यवहार समायोजन गर्छन्, जसले क्षमताहरूको निरन्तर सुधार र परिष्कृततर्फ लैजान्छ।

**यसले व्यवहारमा कसरी काम गर्छ**: एजेन्टहरूले प्रयोगकर्ता प्रतिक्रिया, वातावरणीय डेटा, र कार्य परिणामहरूको विश्लेषण गर्न सक्छन् ताकि उनीहरूको ज्ञान आधार अद्यावधिक गर्न, निर्णय-निर्माण एल्गोरिदम समायोजन गर्न, र समयसँगै प्रदर्शन सुधार गर्न सकियोस्। यो दोहोरिने सिकाइ प्रक्रियाले एजेन्टहरूलाई परिवर्तनशील अवस्थाहरू र प्रयोगकर्ता प्राथमिकताहरूमा अनुकूलन गर्न सक्षम बनाउँछ, समग्र प्रणाली प्रभावकारिता बढाउँछ।

## AutoGen, Semantic Kernel, र Azure AI Agent Service बीच के फरक छ?

यी फ्रेमवर्कहरूको तुलना गर्न धेरै तरिकाहरू छन्, तर तिनीहरूको डिजाइन, क्षमताहरू, र लक्षित प्रयोग केसहरूको सन्दर्भमा केही प्रमुख भिन्नताहरू हेरौं:

## AutoGen

AutoGen माइक्रोसफ्ट रिसर्चको AI Frontiers Lab द्वारा विकसित एक खुला-स्रोत फ्रेमवर्क हो। यो घटनाचालित, वितरित *agentic* अनुप्रयोगहरूमा केन्द्रित छ, जसले धेरै LLMs र SLMs, उपकरणहरू, र उन्नत बहु-एजेन्ट डिजाइन ढाँचाहरू सक्षम बनाउँछ।

AutoGen एजेन्टहरूको कोर अवधारणामा आधारित छ, जुन स्वायत्त इकाइहरू हुन् जसले आफ्नो वातावरणलाई बुझ्न, निर्णय लिन, र विशिष्ट लक्ष्यहरू प्राप्त गर्न कार्य गर्न सक्छन्। एजेन्टहरूले असिन्क्रोनस सन्देशहरूको माध्यमबाट संवाद गर्छन्, जसले तिनीहरूलाई स्वतन्त्र रूपमा र समानान्तरमा काम गर्न अनुमति दिन्छ, प्रणालीको मापनयोग्यता र प्रतिक्रियाशीलता बढाउँछ।
## Azure AI Agent सेवा

Azure AI Agent सेवा हालसालै थपिएको सुविधा हो, जसलाई Microsoft Ignite 2024 मा प्रस्तुत गरिएको थियो। यसले AI एजेन्टहरू विकास र तैनाथ गर्न थप लचिलो मोडेलहरू प्रदान गर्दछ, जस्तै Llama 3, Mistral, र Cohere जस्ता ओपन-सोर्स LLMहरूलाई सिधै कल गर्न।

Azure AI Agent सेवाले बलियो उद्यम सुरक्षा संयन्त्रहरू र डेटा भण्डारण विधिहरू प्रदान गर्दछ, जसले यसलाई उद्यम अनुप्रयोगहरूको लागि उपयुक्त बनाउँछ।

यो सेवा AutoGen र Semantic Kernel जस्ता बहु-एजेन्ट ऑर्केस्ट्रेशन फ्रेमवर्कहरूसँग सहज रूपमा काम गर्दछ।

हाल यो सेवा सार्वजनिक पूर्वावलोकनमा छ र एजेन्ट निर्माणको लागि Python र C# समर्थन गर्दछ।

Semantic Kernel Python प्रयोग गरेर, हामी प्रयोगकर्ताले परिभाषित गरेको प्लगइनको साथमा Azure AI Agent बनाउन सक्छौं:

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

### मुख्य अवधारणाहरू

Azure AI Agent सेवामा निम्न मुख्य अवधारणाहरू छन्:

- **एजेन्ट**। Azure AI Agent सेवा Azure AI Foundry सँग एकीकृत छ। AI Foundry भित्र, AI एजेन्ट "स्मार्ट" माइक्रोसर्भिसको रूपमा कार्य गर्दछ जसले प्रश्नहरूको उत्तर दिन (RAG), कार्यहरू गर्न, वा पूर्ण रूपमा वर्कफ्लोहरू स्वचालित गर्न प्रयोग गर्न सकिन्छ। यसले जेनेरेटिभ AI मोडेलहरूको शक्ति र वास्तविक-विश्व डेटा स्रोतहरूसँग अन्तरक्रिया गर्न अनुमति दिने उपकरणहरूको संयोजन गरेर यो हासिल गर्दछ। यहाँ एउटा एजेन्टको उदाहरण छ:

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    यस उदाहरणमा, `gpt-4o-mini` मोडेल, `my-agent` नाम, र `You are helpful agent` निर्देशनहरूको साथमा एउटा एजेन्ट सिर्जना गरिएको छ। एजेन्टलाई कोड व्याख्या कार्यहरू गर्न उपकरणहरू र स्रोतहरूसँग सुसज्जित गरिएको छ।

- **थ्रेड र सन्देशहरू**। थ्रेड अर्को महत्त्वपूर्ण अवधारणा हो। यसले एजेन्ट र प्रयोगकर्ताबीचको कुराकानी वा अन्तरक्रियालाई प्रतिनिधित्व गर्दछ। थ्रेडहरूले कुराकानीको प्रगति ट्र्याक गर्न, सन्दर्भ जानकारी भण्डारण गर्न, र अन्तरक्रियाको अवस्था व्यवस्थापन गर्न प्रयोग गर्न सकिन्छ। यहाँ थ्रेडको एउटा उदाहरण छ:

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

    माथिको कोडमा, एउटा थ्रेड सिर्जना गरिएको छ। त्यसपछि, थ्रेडमा सन्देश पठाइएको छ। `create_and_process_run` कल गरेर, एजेन्टलाई थ्रेडमा काम गर्न सोधिएको छ। अन्ततः, सन्देशहरू फेच गरिन्छ र एजेन्टको प्रतिक्रिया हेर्नको लागि लग गरिन्छ। सन्देशहरूले प्रयोगकर्ता र एजेन्टबीचको कुराकानीको प्रगति संकेत गर्दछ। यो पनि महत्त्वपूर्ण छ कि सन्देशहरू विभिन्न प्रकारका हुन सक्छन् जस्तै पाठ, छवि, वा फाइल, जुन एजेन्टको कामले उदाहरणका लागि छवि वा पाठ प्रतिक्रिया उत्पादन गरेको छ। एक विकासकर्ताको रूपमा, तपाईंले यो जानकारीलाई थप प्रक्रिया गर्न वा प्रयोगकर्तालाई प्रस्तुत गर्न प्रयोग गर्न सक्नुहुन्छ।

- **अन्य AI फ्रेमवर्कहरूसँग एकीकृत हुन्छ**। Azure AI Agent सेवा AutoGen र Semantic Kernel जस्ता अन्य फ्रेमवर्कहरूसँग अन्तरक्रिया गर्न सक्छ, जसको अर्थ तपाईं आफ्नो अनुप्रयोगको केही भाग यी फ्रेमवर्कहरूमध्ये एकमा निर्माण गर्न सक्नुहुन्छ र उदाहरणका लागि एजेन्ट सेवालाई ऑर्केस्ट्रेटरको रूपमा प्रयोग गर्न सक्नुहुन्छ वा तपाईं सबै कुरा एजेन्ट सेवामा निर्माण गर्न सक्नुहुन्छ।

**प्रयोगका केसहरू**: Azure AI Agent सेवा उद्यम अनुप्रयोगहरूको लागि डिजाइन गरिएको हो जसलाई सुरक्षित, स्केलेबल, र लचिलो AI एजेन्ट तैनाथ आवश्यक छ।

## यी फ्रेमवर्कहरू बीच के फरक छ?

यो सुन्दा धेरै ओभरलैप जस्तो लाग्छ, तर तिनीहरूको डिजाइन, क्षमता, र लक्षित प्रयोगका केसहरूको सन्दर्भमा केही प्रमुख भिन्नताहरू छन्:

- **AutoGen**: बहु-एजेन्ट प्रणालीहरूमा अग्रणी अनुसन्धानमा केन्द्रित प्रयोगात्मक फ्रेमवर्क हो। यो जटिल बहु-एजेन्ट प्रणालीहरू प्रोटोटाइप गर्न र प्रयोग गर्न उत्तम स्थान हो।
- **Semantic Kernel**: उद्यम एजेन्टिक अनुप्रयोगहरू निर्माणको लागि उत्पादन-तयार एजेन्ट लाइब्रेरी हो। यसले घटनाचालित, वितरित एजेन्टिक अनुप्रयोगहरूमा ध्यान केन्द्रित गर्दछ, बहु LLMs र SLMs, उपकरणहरू, र एकल/बहु-एजेन्ट डिजाइन ढाँचाहरू सक्षम गर्दछ।
- **Azure AI Agent सेवा**: Azure Foundry मा एजेन्टहरूको लागि प्लेटफर्म र तैनाथ सेवा हो। यसले Azure Foundry द्वारा समर्थित सेवाहरू जस्तै Azure OpenAI, Azure AI Search, Bing Search र कोड कार्यान्वयनमा कनेक्टिविटी निर्माणको प्रस्ताव गर्दछ।

अझै पनि कुन छनोट गर्ने निश्चित छैन?

### प्रयोगका केसहरू

आउनुहोस्, केही सामान्य प्रयोगका केसहरू हेरेर तपाईंलाई मद्दत गर्ने प्रयास गरौं:

> प्रश्न: म प्रयोग गर्दैछु, सिक्दैछु र प्रमाण-अवधारणा एजेन्ट अनुप्रयोगहरू निर्माण गर्दैछु, र म छिटो निर्माण र प्रयोग गर्न सक्षम हुन चाहन्छु।

> उत्तर: AutoGen यस परिदृश्यको लागि राम्रो विकल्प हुनेछ, किनकि यसले घटनाचालित, वितरित एजेन्टिक अनुप्रयोगहरूमा ध्यान केन्द्रित गर्दछ र उन्नत बहु-एजेन्ट डिजाइन ढाँचाहरूलाई समर्थन गर्दछ।

> प्रश्न: यस प्रयोगका केसको लागि Semantic Kernel र Azure AI Agent सेवाको तुलनामा AutoGen किन राम्रो विकल्प हो?

> उत्तर: AutoGen विशेष रूपमा घटनाचालित, वितरित एजेन्टिक अनुप्रयोगहरूको लागि डिजाइन गरिएको हो, जसले यसलाई कोड जेनेरेशन र डेटा विश्लेषण कार्यहरू स्वचालित गर्न राम्रो बनाउँछ। यसले जटिल बहु-एजेन्ट प्रणालीहरू कुशलतापूर्वक निर्माण गर्न आवश्यक उपकरणहरू र क्षमताहरू प्रदान गर्दछ।

> प्रश्न: Azure AI Agent सेवा पनि यहाँ काम गर्न सक्छ, यसमा कोड जेनेरेशन र अन्य उपकरणहरू छन्, हैन?

> उत्तर: हो, Azure AI Agent सेवा एजेन्टहरूको लागि प्लेटफर्म सेवा हो र बहु मोडेलहरू, Azure AI Search, Bing Search र Azure Functions को लागि निर्मित क्षमताहरू थप गर्दछ। यसले Foundry Portal मा तपाईंको एजेन्टहरू निर्माण गर्न र तिनीहरूलाई स्केलमा तैनाथ गर्न सजिलो बनाउँछ।

> प्रश्न: म अझै पनि अलमलमा छु, मलाई एउटा विकल्प मात्र दिनुहोस्।

> उत्तर: एउटा उत्कृष्ट विकल्प Semantic Kernel मा तपाईंको अनुप्रयोग निर्माण गर्नु हो र त्यसपछि Azure AI Agent सेवा प्रयोग गरेर तपाईंको एजेन्ट तैनाथ गर्नु हो। यसले तपाईंलाई तपाईंको एजेन्टहरू सजिलैसँग स्थायी बनाउन अनुमति दिन्छ जबकि Semantic Kernel मा बहु-एजेन्ट प्रणालीहरू निर्माण गर्ने शक्ति प्रयोग गर्दै। थप रूपमा, Semantic Kernel मा AutoGen को कनेक्टर छ, जसले यी फ्रेमवर्कहरूलाई सँगै प्रयोग गर्न सजिलो बनाउँछ।

आउनुहोस्, मुख्य भिन्नताहरूलाई तालिकामा संक्षेपमा प्रस्तुत गरौं:

| फ्रेमवर्क | ध्यान केन्द्रित | मुख्य अवधारणाहरू | प्रयोगका केसहरू |
| --- | --- | --- | --- |
| AutoGen | घटनाचालित, वितरित एजेन्टिक अनुप्रयोगहरू | एजेन्टहरू, व्यक्तित्वहरू, कार्यहरू, डेटा | कोड जेनेरेशन, डेटा विश्लेषण कार्यहरू |
| Semantic Kernel | मानव-जस्तो पाठ सामग्री बुझ्ने र उत्पन्न गर्ने | एजेन्टहरू, मोड्युलर कम्पोनेन्टहरू, सहकार्य | प्राकृतिक भाषा बुझाइ, सामग्री उत्पन्न |
| Azure AI Agent सेवा | लचिलो मोडेलहरू, उद्यम सुरक्षा, कोड जेनेरेशन, उपकरण कलिंग | मोड्युलरिटी, सहकार्य, प्रक्रिया ऑर्केस्ट्रेशन | सुरक्षित, स्केलेबल, र लचिलो AI एजेन्ट तैनाथ |

प्रत्येक फ्रेमवर्कको आदर्श प्रयोगका केस के हो?

## के म मेरो विद्यमान Azure इकोसिस्टम उपकरणहरू सिधै एकीकृत गर्न सक्छु, वा मलाई स्वतन्त्र समाधानहरू चाहिन्छ?

उत्तर हो, तपाईं Azure AI Agent सेवासँग विशेष रूपमा आफ्नो विद्यमान Azure इकोसिस्टम उपकरणहरू सिधै एकीकृत गर्न सक्नुहुन्छ, किनकि यसलाई अन्य Azure सेवाहरूको साथ सहज रूपमा काम गर्न निर्माण गरिएको छ। उदाहरणका लागि, तपाईं Bing, Azure AI Search, र Azure Functions एकीकृत गर्न सक्नुहुन्छ। Azure AI Foundry सँग पनि गहिरो एकीकरण छ।

AutoGen र Semantic Kernel को लागि, तपाईं Azure सेवाहरूलाई पनि एकीकृत गर्न सक्नुहुन्छ, तर यसले तपाईंलाई तपाईंको कोडबाट Azure सेवाहरू कल गर्न आवश्यक हुन सक्छ। अर्को तरिका भनेको Azure SDKs प्रयोग गरेर तपाईंको एजेन्टहरूबाट Azure सेवाहरूको साथ अन्तरक्रिया गर्नु हो। थप रूपमा, जस्तै उल्लेख गरिएको थियो, तपाईं AutoGen वा Semantic Kernel मा निर्माण गरिएको तपाईंको एजेन्टहरूको लागि ऑर्केस्ट्रेटरको रूपमा Azure AI Agent सेवा प्रयोग गर्न सक्नुहुन्छ, जसले Azure इकोसिस्टममा सजिलो पहुँच प्रदान गर्दछ।

### AI एजेन्ट फ्रेमवर्कहरूको बारेमा थप प्रश्नहरू छन्?

[Azure AI Foundry Discord](https://aka.ms/ai-agents/discord) मा सामेल हुनुहोस् अन्य सिक्नेहरूलाई भेट्न, कार्यालय समयमा भाग लिन र तपाईंको AI एजेन्टहरूको प्रश्नहरूको उत्तर पाउन।

## सन्दर्भहरू

## अघिल्लो पाठ

[AI एजेन्टहरू र एजेन्ट प्रयोगका केसहरूको परिचय](../01-intro-to-ai-agents/README.md)

## अर्को पाठ

[एजेन्टिक डिजाइन ढाँचाहरू बुझ्दै](../03-agentic-design-patterns/README.md)

---

**अस्वीकरण**:  
यो दस्तावेज़ AI अनुवाद सेवा [Co-op Translator](https://github.com/Azure/co-op-translator) प्रयोग गरेर अनुवाद गरिएको छ। हामी शुद्धताको लागि प्रयास गर्छौं, तर कृपया ध्यान दिनुहोस् कि स्वचालित अनुवादहरूमा त्रुटि वा अशुद्धता हुन सक्छ। यसको मूल भाषा मा रहेको मूल दस्तावेज़लाई आधिकारिक स्रोत मानिनुपर्छ। महत्वपूर्ण जानकारीको लागि, व्यावसायिक मानव अनुवाद सिफारिस गरिन्छ। यस अनुवादको प्रयोगबाट उत्पन्न हुने कुनै पनि गलतफहमी वा गलत व्याख्याको लागि हामी जिम्मेवार हुने छैनौं।