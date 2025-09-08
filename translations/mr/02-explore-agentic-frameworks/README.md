<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-29T10:07:19+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "mr"
}
-->
[![Exploring AI Agent Frameworks](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.mr.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(वरील प्रतिमेवर क्लिक करून या धड्याचा व्हिडिओ पहा)_

# AI एजंट फ्रेमवर्क्सचा अभ्यास करा

AI एजंट फ्रेमवर्क्स हे सॉफ्टवेअर प्लॅटफॉर्म आहेत जे AI एजंट्स तयार करणे, तैनात करणे आणि व्यवस्थापित करणे सुलभ करतात. हे फ्रेमवर्क्स विकसकांना पूर्व-निर्मित घटक, संकल्पना आणि साधने प्रदान करतात, ज्यामुळे जटिल AI प्रणालींच्या विकासात सुलभता येते.

हे फ्रेमवर्क्स AI एजंट विकासातील सामान्य आव्हानांसाठी प्रमाणित दृष्टिकोन प्रदान करून विकसकांना त्यांच्या अनुप्रयोगांच्या अद्वितीय पैलूंवर लक्ष केंद्रित करण्यास मदत करतात. ते AI प्रणाली तयार करण्यात स्केलेबिलिटी, प्रवेशयोग्यता आणि कार्यक्षमता वाढवतात.

## परिचय

या धड्यात आपण शिकणार आहोत:

- AI एजंट फ्रेमवर्क्स म्हणजे काय आणि ते विकसकांना काय साध्य करण्यास सक्षम करतात?
- संघ हे फ्रेमवर्क्स कसे वापरून जलद प्रोटोटाइप तयार करू शकतात, पुनरावृत्ती करू शकतात आणि त्यांच्या एजंटच्या क्षमतांमध्ये सुधारणा करू शकतात?
- Microsoft ने तयार केलेल्या फ्रेमवर्क्स आणि टूल्समधील फरक काय आहेत?
- मी माझ्या विद्यमान Azure इकोसिस्टम टूल्स थेट समाकलित करू शकतो का, की मला स्वतंत्र सोल्यूशन्सची आवश्यकता आहे?
- Azure AI Agents सेवा म्हणजे काय आणि ती मला कशी मदत करते?

## शिकण्याची उद्दिष्टे

या धड्याचे उद्दिष्टे तुम्हाला समजून घेण्यास मदत करणे आहेत:

- AI एजंट फ्रेमवर्क्सचा AI विकासातील महत्त्वाचा रोल.
- AI एजंट फ्रेमवर्क्सचा उपयोग करून बुद्धिमान एजंट्स कसे तयार करायचे.
- AI एजंट फ्रेमवर्क्सद्वारे सक्षम केलेल्या प्रमुख क्षमता.
- AutoGen, Semantic Kernel, आणि Azure AI Agent Service यामधील फरक.

## AI एजंट फ्रेमवर्क्स म्हणजे काय आणि ते विकसकांना काय साध्य करण्यास सक्षम करतात?

पारंपरिक AI फ्रेमवर्क्स तुमच्या अॅप्समध्ये AI समाकलित करण्यात आणि खालील प्रकारे त्यांना अधिक चांगले बनवण्यात मदत करू शकतात:

- **वैयक्तिकरण**: AI वापरकर्त्याच्या वर्तनाचा आणि प्राधान्यांचा विश्लेषण करून वैयक्तिक शिफारसी, सामग्री आणि अनुभव प्रदान करू शकतो.
उदाहरण: Netflix सारख्या स्ट्रीमिंग सेवांचा वापर AI करून पाहण्याच्या इतिहासावर आधारित चित्रपट आणि शो सुचवण्यासाठी केला जातो, ज्यामुळे वापरकर्त्यांचा सहभाग आणि समाधान वाढते.
- **स्वयंचलन आणि कार्यक्षमता**: AI पुनरावृत्ती होणाऱ्या कार्यांचे स्वयंचलन करू शकतो, कार्यप्रवाह सुव्यवस्थित करू शकतो आणि कार्यक्षमता सुधारू शकतो.
उदाहरण: ग्राहक सेवा अॅप्स AI-चालित चॅटबॉट्सचा वापर सामान्य चौकशी हाताळण्यासाठी करतात, प्रतिसाद वेळ कमी करतात आणि अधिक जटिल समस्यांसाठी मानवी एजंट्सना मोकळे करतात.
- **वाढलेला वापरकर्ता अनुभव**: AI आवाज ओळख, नैसर्गिक भाषा प्रक्रिया आणि प्रेडिक्टिव्ह टेक्स्ट यासारख्या बुद्धिमान वैशिष्ट्यांद्वारे एकूणच वापरकर्ता अनुभव सुधारू शकतो.
उदाहरण: Siri आणि Google Assistant सारखे व्हर्च्युअल सहाय्यक AI चा वापर करून आवाज आदेश समजून घेतात आणि प्रतिसाद देतात, ज्यामुळे वापरकर्त्यांना त्यांच्या डिव्हाइसशी संवाद साधणे सोपे होते.

### हे सर्व छान वाटते, मग AI एजंट फ्रेमवर्कची गरज का आहे?

AI एजंट फ्रेमवर्क्स हे केवळ AI फ्रेमवर्क्सपेक्षा अधिक काहीतरी दर्शवतात. ते बुद्धिमान एजंट्स तयार करण्यासाठी डिझाइन केले आहेत जे वापरकर्त्यांसोबत, इतर एजंट्ससोबत आणि विशिष्ट उद्दिष्टे साध्य करण्यासाठी वातावरणाशी संवाद साधू शकतात. हे एजंट्स स्वायत्त वर्तन प्रदर्शित करू शकतात, निर्णय घेऊ शकतात आणि बदलत्या परिस्थितीशी जुळवून घेऊ शकतात. AI एजंट फ्रेमवर्क्सद्वारे सक्षम केलेल्या काही प्रमुख क्षमतांकडे पाहूया:

- **एजंट्समधील सहकार्य आणि समन्वय**: अनेक AI एजंट्स तयार करण्यास सक्षम करा जे एकत्र काम करू शकतात, संवाद साधू शकतात आणि जटिल कार्ये सोडवण्यासाठी समन्वय साधू शकतात.
- **कार्य स्वयंचलन आणि व्यवस्थापन**: मल्टी-स्टेप कार्यप्रवाहांचे स्वयंचलन, कार्य प्रतिनिधीकरण आणि एजंट्समधील डायनॅमिक कार्य व्यवस्थापनासाठी यंत्रणा प्रदान करा.
- **संदर्भात्मक समज आणि अनुकूलन**: एजंट्सना संदर्भ समजून घेण्याची, बदलत्या वातावरणाशी जुळवून घेण्याची आणि रिअल-टाइम माहितीच्या आधारे निर्णय घेण्याची क्षमता द्या.

थोडक्यात, एजंट्स तुम्हाला अधिक करण्यास, स्वयंचलन पुढील स्तरावर नेण्यास, अधिक बुद्धिमान प्रणाली तयार करण्यास सक्षम करतात ज्या त्यांच्या वातावरणातून शिकू शकतात आणि जुळवून घेऊ शकतात.

## एजंटच्या क्षमतांमध्ये जलद प्रोटोटाइप तयार करणे, पुनरावृत्ती करणे आणि सुधारणा कशी करावी?

हे एक वेगाने बदलणारे क्षेत्र आहे, परंतु बहुतेक AI एजंट फ्रेमवर्क्समध्ये काही गोष्टी सामान्य आहेत ज्या तुम्हाला जलद प्रोटोटाइप तयार करण्यात आणि पुनरावृत्ती करण्यात मदत करू शकतात, म्हणजेच मॉड्यूलर घटक, सहकार्यात्मक साधने आणि रिअल-टाइम शिक्षण. चला यामध्ये खोलवर जाऊया:

- **मॉड्यूलर घटकांचा वापर करा**: AI SDKs पूर्व-निर्मित घटक प्रदान करतात जसे की AI आणि मेमरी कनेक्टर्स, नैसर्गिक भाषेचा वापर करून फंक्शन कॉलिंग किंवा कोड प्लगइन्स, प्रॉम्प्ट टेम्पलेट्स आणि बरेच काही.
- **सहकार्यात्मक साधनांचा लाभ घ्या**: विशिष्ट भूमिका आणि कार्यांसह एजंट्स डिझाइन करा, ज्यामुळे त्यांना सहकार्यात्मक कार्यप्रवाहांची चाचणी घेता येईल आणि त्यात सुधारणा करता येईल.
- **रिअल-टाइममध्ये शिका**: फीडबॅक लूप्स अंमलात आणा जिथे एजंट्स परस्परसंवादांमधून शिकतात आणि त्यांचे वर्तन डायनॅमिकरीत्या समायोजित करतात.

### मॉड्यूलर घटकांचा वापर करा

Microsoft Semantic Kernel आणि LangChain सारखे SDKs पूर्व-निर्मित घटक प्रदान करतात जसे की AI कनेक्टर्स, प्रॉम्प्ट टेम्पलेट्स आणि मेमरी व्यवस्थापन.

**संघ हे कसे वापरू शकतात**: संघ हे घटक जलद कार्यशील प्रोटोटाइप तयार करण्यासाठी एकत्र करू शकतात, ज्यामुळे सुरुवातीपासून सुरुवात न करता जलद प्रयोग आणि पुनरावृत्ती होऊ शकते.

**हे प्रत्यक्षात कसे कार्य करते**: तुम्ही वापरकर्त्याच्या इनपुटमधून माहिती काढण्यासाठी पूर्व-निर्मित पार्सर, डेटा साठवण्यासाठी आणि पुनर्प्राप्त करण्यासाठी मेमरी मॉड्यूल आणि वापरकर्त्यांसोबत संवाद साधण्यासाठी प्रॉम्प्ट जनरेटर वापरू शकता, हे सर्व घटक सुरुवातीपासून तयार करण्याची गरज नाही.

**उदाहरण कोड**. चला पाहूया की तुम्ही Semantic Kernel Python आणि .Net सह पूर्व-निर्मित AI कनेक्टरचा वापर करून वापरकर्त्याच्या इनपुटला प्रतिसाद देण्यासाठी मॉडेल कसे वापरू शकता:

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

या उदाहरणातून तुम्हाला दिसेल की तुम्ही वापरकर्त्याच्या इनपुटमधून मूळ, गंतव्यस्थान आणि फ्लाइट बुकिंग विनंतीची तारीख यासारखी महत्त्वाची माहिती कशी काढू शकता. हा मॉड्यूलर दृष्टिकोन तुम्हाला उच्च-स्तरीय लॉजिकवर लक्ष केंद्रित करण्यास अनुमती देतो.

### सहकार्यात्मक साधनांचा लाभ घ्या

CrewAI, Microsoft AutoGen, आणि Semantic Kernel सारखी फ्रेमवर्क्स अनेक एजंट्स तयार करण्यास सुलभ करतात जे एकत्र काम करू शकतात.

**संघ हे कसे वापरू शकतात**: संघ विशिष्ट भूमिका आणि कार्यांसह एजंट्स डिझाइन करू शकतात, ज्यामुळे त्यांना सहकार्यात्मक कार्यप्रवाहांची चाचणी घेता येईल आणि सुधारणा करता येईल.

**हे प्रत्यक्षात कसे कार्य करते**: तुम्ही एजंट्सची एक टीम तयार करू शकता जिथे प्रत्येक एजंटची डेटा पुनर्प्राप्ती, विश्लेषण किंवा निर्णय घेणे यासारखी एक विशेष कार्ये असतात. हे एजंट्स माहिती सामायिक करू शकतात आणि वापरकर्त्याच्या चौकशीला उत्तर देण्यासाठी किंवा कार्य पूर्ण करण्यासाठी एकत्र काम करू शकतात.

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

मागील कोडमध्ये तुम्ही पाहू शकता की डेटा विश्लेषणासाठी अनेक एजंट्स एकत्र काम करत आहेत. प्रत्येक एजंट एक विशिष्ट कार्य करतो, आणि कार्य इच्छित परिणाम साध्य करण्यासाठी एजंट्सचे समन्वय साधून अंमलात आणले जाते. समर्पित एजंट्स तयार करून, कार्यक्षमता आणि कार्यक्षमता सुधारली जाऊ शकते.

### रिअल-टाइममध्ये शिका

प्रगत फ्रेमवर्क्स रिअल-टाइम संदर्भ समजून घेणे आणि अनुकूलन करण्यासाठी क्षमता प्रदान करतात.

**संघ हे कसे वापरू शकतात**: संघ फीडबॅक लूप्स अंमलात आणू शकतात जिथे एजंट्स परस्परसंवादांमधून शिकतात आणि त्यांचे वर्तन डायनॅमिकरीत्या समायोजित करतात, ज्यामुळे सतत सुधारणा आणि क्षमतांची परिष्कृती होते.

**हे प्रत्यक्षात कसे कार्य करते**: एजंट्स वापरकर्त्याच्या फीडबॅक, पर्यावरणीय डेटा आणि कार्य परिणामांचे विश्लेषण करू शकतात, त्यांचे ज्ञान अद्यतनित करू शकतात, निर्णय घेण्याचे अल्गोरिदम समायोजित करू शकतात आणि वेळोवेळी कार्यप्रदर्शन सुधारू शकतात. हा पुनरावृत्ती शिकण्याचा प्रक्रिया एजंट्सना बदलत्या परिस्थितीशी जुळवून घेण्यास आणि वापरकर्त्याच्या प्राधान्यांशी जुळवून घेण्यास सक्षम करते, ज्यामुळे एकूणच प्रणालीची कार्यक्षमता वाढते.

## AutoGen, Semantic Kernel आणि Azure AI Agent Service यामधील फरक काय आहेत?

या फ्रेमवर्क्सची तुलना करण्याचे अनेक मार्ग आहेत, परंतु त्यांच्या डिझाइन, क्षमता आणि लक्ष्यित उपयोग प्रकरणांच्या दृष्टीने काही प्रमुख फरक पाहूया:

## AutoGen

AutoGen हे Microsoft Research च्या AI Frontiers Lab ने विकसित केलेले एक ओपन-सोर्स फ्रेमवर्क आहे. हे इव्हेंट-ड्रिव्हन, वितरित *agentic* अनुप्रयोगांवर लक्ष केंद्रित करते, ज्यामुळे अनेक LLMs आणि SLMs, साधने आणि प्रगत मल्टी-एजंट डिझाइन पॅटर्न सक्षम होतात.

AutoGen एजंट्स या मुख्य संकल्पनेभोवती तयार केले आहे, जे स्वायत्त घटक आहेत जे त्यांच्या वातावरणाचे आकलन करू शकतात, निर्णय घेऊ शकतात आणि विशिष्ट उद्दिष्टे साध्य करण्यासाठी कृती करू शकतात. एजंट्स असिंक्रोनस संदेशांद्वारे संवाद साधतात, ज्यामुळे ते स्वतंत्रपणे आणि समांतरपणे कार्य करू शकतात, प्रणालीची स्केलेबिलिटी आणि प्रतिसादक्षमता वाढते.
तर, हे Semantic Kernel फ्रेमवर्कचे मूलभूत ज्ञान आहे, आता Agent Framework बद्दल काय?

## Azure AI Agent Service

Azure AI Agent Service ही एक नवीन सेवा आहे, जी Microsoft Ignite 2024 मध्ये सादर करण्यात आली. ही सेवा AI एजंट्स विकसित करण्यासाठी आणि तैनात करण्यासाठी अधिक लवचिक मॉडेल्ससह कार्य करण्याची परवानगी देते, जसे की Llama 3, Mistral, आणि Cohere सारख्या ओपन-सोर्स LLMs थेट कॉल करणे.

Azure AI Agent Service मजबूत एंटरप्राइझ सुरक्षा यंत्रणा आणि डेटा संग्रहण पद्धती प्रदान करते, ज्यामुळे ती एंटरप्राइझ अनुप्रयोगांसाठी योग्य ठरते.

ही सेवा AutoGen आणि Semantic Kernel सारख्या मल्टी-एजंट ऑर्केस्ट्रेशन फ्रेमवर्कसह सहजपणे कार्य करते.

सध्या ही सेवा Public Preview मध्ये आहे आणि एजंट्स तयार करण्यासाठी Python आणि C# ला समर्थन देते.

Semantic Kernel Python वापरून, आपण वापरकर्ता-परिभाषित प्लगइनसह Azure AI Agent तयार करू शकतो:

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

### मुख्य संकल्पना

Azure AI Agent Service मध्ये खालील मुख्य संकल्पना आहेत:

- **Agent**. Azure AI Agent Service Azure AI Foundry सह एकत्रित होते. AI Foundry मध्ये, AI Agent एक "स्मार्ट" मायक्रोसर्विस म्हणून कार्य करते जी प्रश्नांची उत्तरे देण्यासाठी (RAG), कृती करण्यासाठी किंवा पूर्णपणे वर्कफ्लो स्वयंचलित करण्यासाठी वापरली जाऊ शकते. हे जनरेटिव्ह AI मॉडेल्सच्या शक्तीला वास्तविक डेटा स्रोतांशी संवाद साधण्यास सक्षम करणाऱ्या साधनांसह एकत्र करून साध्य करते. एजंटचे एक उदाहरण येथे आहे:

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    या उदाहरणात, `gpt-4o-mini` मॉडेल, `my-agent` नाव, आणि `You are helpful agent` सूचना असलेला एजंट तयार केला जातो. कोड इंटरप्रिटेशन कार्ये करण्यासाठी एजंट साधने आणि संसाधनांनी सुसज्ज आहे.

- **Thread आणि Messages**. थ्रेड ही आणखी एक महत्त्वाची संकल्पना आहे. ती एजंट आणि वापरकर्त्यादरम्यान संभाषण किंवा संवादाचे प्रतिनिधित्व करते. थ्रेड्स संभाषणाची प्रगती ट्रॅक करण्यासाठी, संदर्भ माहिती संग्रहित करण्यासाठी, आणि संवादाची स्थिती व्यवस्थापित करण्यासाठी वापरली जाऊ शकते. थ्रेडचे एक उदाहरण येथे आहे:

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

    मागील कोडमध्ये, एक थ्रेड तयार केला जातो. त्यानंतर, थ्रेडला एक संदेश पाठवला जातो. `create_and_process_run` कॉल करून, एजंटला थ्रेडवर काम करण्यास सांगितले जाते. शेवटी, संदेश मिळवले जातात आणि एजंटच्या प्रतिसादाचे लॉगिंग केले जाते. संदेश वापरकर्ता आणि एजंटमधील संभाषणाची प्रगती दर्शवतात. हे देखील महत्त्वाचे आहे की संदेश वेगवेगळ्या प्रकारचे असू शकतात जसे की मजकूर, प्रतिमा, किंवा फाइल, म्हणजे एजंटच्या कार्यामुळे उदाहरणार्थ प्रतिमा किंवा मजकूर प्रतिसाद तयार झाला आहे. एक विकसक म्हणून, तुम्ही नंतर या माहितीचा वापर प्रतिसाद पुढे प्रक्रिया करण्यासाठी किंवा वापरकर्त्याला सादर करण्यासाठी करू शकता.

- **इतर AI फ्रेमवर्कसह एकत्रित होते**. Azure AI Agent Service AutoGen आणि Semantic Kernel सारख्या इतर फ्रेमवर्कसह संवाद साधू शकते, म्हणजे तुम्ही तुमच्या अॅपचा काही भाग या फ्रेमवर्कमध्ये तयार करू शकता आणि उदाहरणार्थ Agent Service चा ऑर्केस्ट्रेटर म्हणून वापर करू शकता किंवा तुम्ही सर्वकाही Agent Service मध्ये तयार करू शकता.

**वापर प्रकरणे**: Azure AI Agent Service सुरक्षित, स्केलेबल, आणि लवचिक AI एजंट तैनातीसाठी डिझाइन केले आहे.

## या फ्रेमवर्क्समध्ये काय फरक आहे?

हे फ्रेमवर्क्समध्ये बरेच साम्य आहे असे वाटते, परंतु त्यांच्या डिझाइन, क्षमता, आणि लक्ष्यित वापर प्रकरणांमध्ये काही महत्त्वाचे फरक आहेत:

- **AutoGen**: मल्टी-एजंट सिस्टीम्सवरील अत्याधुनिक संशोधनावर लक्ष केंद्रित करणारे प्रयोग फ्रेमवर्क आहे. जटिल मल्टी-एजंट सिस्टीम्सची प्रोटोटाइप तयार करण्यासाठी आणि प्रयोग करण्यासाठी सर्वोत्तम जागा आहे.
- **Semantic Kernel**: एंटरप्राइझ एजंटिक अनुप्रयोग तयार करण्यासाठी उत्पादन-तयार एजंट लायब्ररी आहे. इव्हेंट-ड्रिव्हन, वितरित एजंटिक अनुप्रयोगांवर लक्ष केंद्रित करते, अनेक LLMs आणि SLMs, साधने, आणि सिंगल/मल्टी-एजंट डिझाइन पॅटर्न सक्षम करते.
- **Azure AI Agent Service**: Azure Foundry मध्ये एजंट्ससाठी एक प्लॅटफॉर्म आणि तैनाती सेवा आहे. Azure OpenAI, Azure AI Search, Bing Search आणि कोड कार्यान्वयनास समर्थन देणाऱ्या सेवांशी कनेक्टिव्हिटी तयार करण्याची ऑफर देते.

तुम्हाला अजूनही कोणते निवडायचे ते ठरवता येत नाही का?

### वापर प्रकरणे

चला काही सामान्य वापर प्रकरणांमधून जाऊन तुम्हाला मदत करूया:

> Q: मी प्रयोग करत आहे, शिकत आहे आणि प्रूफ-ऑफ-कॉन्सेप्ट एजंट अनुप्रयोग तयार करत आहे, आणि मला जलदपणे तयार करणे आणि प्रयोग करणे शक्य व्हावे असे वाटते
>

>A: AutoGen या परिस्थितीसाठी चांगला पर्याय असेल, कारण तो इव्हेंट-ड्रिव्हन, वितरित एजंटिक अनुप्रयोगांवर लक्ष केंद्रित करतो आणि प्रगत मल्टी-एजंट डिझाइन पॅटर्नसाठी समर्थन प्रदान करतो.

> Q: या वापर प्रकरणासाठी Semantic Kernel आणि Azure AI Agent Service पेक्षा AutoGen चांगला पर्याय का आहे?
>
> A: AutoGen विशेषतः इव्हेंट-ड्रिव्हन, वितरित एजंटिक अनुप्रयोगांसाठी डिझाइन केले आहे, ज्यामुळे कोड जनरेशन आणि डेटा विश्लेषण कार्ये स्वयंचलित करण्यासाठी ते योग्य आहे. हे जटिल मल्टी-एजंट सिस्टीम्स कार्यक्षमतेने तयार करण्यासाठी आवश्यक साधने आणि क्षमता प्रदान करते.

>Q: Azure AI Agent Service येथे देखील कार्य करू शकते, त्यात कोड जनरेशन आणि अधिकसाठी साधने आहेत का?
>
> A: होय, Azure AI Agent Service ही एजंट्ससाठी एक प्लॅटफॉर्म सेवा आहे आणि अनेक मॉडेल्स, Azure AI Search, Bing Search आणि Azure Functions साठी अंगभूत क्षमता जोडते. हे Foundry Portal मध्ये तुमचे एजंट्स तयार करणे आणि मोठ्या प्रमाणावर तैनात करणे सोपे करते.

> Q: मला अजूनही गोंधळ आहे, फक्त एक पर्याय द्या
>
> A: एक उत्तम पर्याय म्हणजे तुमचा अनुप्रयोग Semantic Kernel मध्ये प्रथम तयार करणे आणि नंतर Azure AI Agent Service वापरून तुमचा एजंट तैनात करणे. या दृष्टिकोनामुळे तुम्हाला तुमचे एजंट्स सहजपणे टिकवता येतील आणि Semantic Kernel मध्ये मल्टी-एजंट सिस्टीम्स तयार करण्याची क्षमता मिळेल. याशिवाय, Semantic Kernel मध्ये AutoGen मध्ये कनेक्टर आहे, ज्यामुळे दोन्ही फ्रेमवर्क्स एकत्र वापरणे सोपे होते.

चला मुख्य फरक एका टेबलमध्ये संक्षेप करूया:

| फ्रेमवर्क | लक्ष केंद्रित | मुख्य संकल्पना | वापर प्रकरणे |
| --- | --- | --- | --- |
| AutoGen | इव्हेंट-ड्रिव्हन, वितरित एजंटिक अनुप्रयोग | एजंट्स, पर्सोनाज, फंक्शन्स, डेटा | कोड जनरेशन, डेटा विश्लेषण कार्ये |
| Semantic Kernel | मानवीसारखे मजकूर सामग्री समजून घेणे आणि तयार करणे | एजंट्स, मॉड्युलर घटक, सहयोग | नैसर्गिक भाषा समजून घेणे, सामग्री निर्मिती |
| Azure AI Agent Service | लवचिक मॉडेल्स, एंटरप्राइझ सुरक्षा, कोड जनरेशन, टूल कॉलिंग | मॉड्युलरिटी, सहयोग, प्रक्रिया ऑर्केस्ट्रेशन | सुरक्षित, स्केलेबल, आणि लवचिक AI एजंट तैनाती |

प्रत्येक फ्रेमवर्कसाठी आदर्श वापर प्रकरण काय आहे?

## मी माझ्या विद्यमान Azure इकोसिस्टम टूल्स थेट एकत्रित करू शकतो का, किंवा मला स्वतंत्र सोल्यूशन्सची आवश्यकता आहे?

उत्तर होय आहे, तुम्ही Azure AI Agent Service सह तुमच्या विद्यमान Azure इकोसिस्टम टूल्स थेट एकत्रित करू शकता, विशेषतः कारण ती इतर Azure सेवांसह सहजपणे कार्य करण्यासाठी तयार केली गेली आहे. उदाहरणार्थ, तुम्ही Bing, Azure AI Search, आणि Azure Functions एकत्रित करू शकता. Azure AI Foundry सह सखोल एकत्रीकरण देखील आहे.

AutoGen आणि Semantic Kernel साठी, तुम्ही Azure सेवांसह एकत्रित करू शकता, परंतु तुम्हाला तुमच्या कोडमधून Azure सेवांना कॉल करावे लागेल. एकत्रित करण्याचा आणखी एक मार्ग म्हणजे Azure SDKs वापरून तुमच्या एजंट्समधून Azure सेवांसह संवाद साधणे. याशिवाय, जसे नमूद केले गेले, तुम्ही AutoGen किंवा Semantic Kernel मध्ये तयार केलेल्या एजंट्ससाठी Azure AI Agent Service ऑर्केस्ट्रेटर म्हणून वापरू शकता, ज्यामुळे Azure इकोसिस्टममध्ये सहज प्रवेश मिळतो.

### AI Agent Frameworks बद्दल अधिक प्रश्न आहेत का?

[Azure AI Foundry Discord](https://aka.ms/ai-agents/discord) मध्ये सामील व्हा, इतर शिकणाऱ्यांशी भेटा, ऑफिस तासांमध्ये सहभागी व्हा आणि तुमचे AI Agents संबंधित प्रश्न विचारून उत्तरे मिळवा.

## संदर्भ

- 

## मागील धडा

[AI एजंट्स आणि एजंट वापर प्रकरणांची ओळख](../01-intro-to-ai-agents/README.md)

## पुढील धडा

[एजंटिक डिझाइन पॅटर्न्स समजून घेणे](../03-agentic-design-patterns/README.md)

---

**अस्वीकरण**:  
हा दस्तऐवज AI भाषांतर सेवा [Co-op Translator](https://github.com/Azure/co-op-translator) चा वापर करून भाषांतरित करण्यात आला आहे. आम्ही अचूकतेसाठी प्रयत्नशील असलो तरी, कृपया लक्षात घ्या की स्वयंचलित भाषांतरांमध्ये त्रुटी किंवा अचूकतेचा अभाव असू शकतो. मूळ भाषेतील दस्तऐवज हा अधिकृत स्रोत मानला जावा. महत्त्वाच्या माहितीसाठी व्यावसायिक मानवी भाषांतराची शिफारस केली जाते. या भाषांतराचा वापर केल्यामुळे उद्भवणाऱ्या कोणत्याही गैरसमज किंवा चुकीच्या अर्थासाठी आम्ही जबाबदार राहणार नाही.