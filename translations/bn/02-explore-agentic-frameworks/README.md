<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-29T12:18:27+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "bn"
}
-->
[![এআই এজেন্ট ফ্রেমওয়ার্ক অন্বেষণ](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.bn.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(উপরের ছবিতে ক্লিক করে এই পাঠের ভিডিও দেখুন)_

# এআই এজেন্ট ফ্রেমওয়ার্ক অন্বেষণ

এআই এজেন্ট ফ্রেমওয়ার্ক হলো সফটওয়্যার প্ল্যাটফর্ম যা এআই এজেন্ট তৈরি, স্থাপন এবং পরিচালনা সহজতর করার জন্য ডিজাইন করা হয়েছে। এই ফ্রেমওয়ার্কগুলো ডেভেলপারদের জন্য প্রি-বিল্ট কম্পোনেন্ট, অ্যাবস্ট্রাকশন এবং টুল সরবরাহ করে যা জটিল এআই সিস্টেমের উন্নয়নকে সহজ করে।

এই ফ্রেমওয়ার্কগুলো ডেভেলপারদের তাদের অ্যাপ্লিকেশনের অনন্য দিকগুলোর উপর মনোযোগ কেন্দ্রীভূত করতে সাহায্য করে, এআই এজেন্ট উন্নয়নের সাধারণ চ্যালেঞ্জগুলোর জন্য মানসম্মত পদ্ধতি প্রদান করে। এগুলো এআই সিস্টেম তৈরিতে স্কেলেবিলিটি, অ্যাক্সেসিবিলিটি এবং দক্ষতা বৃদ্ধি করে।

## পরিচিতি

এই পাঠে আলোচনা করা হবে:

- এআই এজেন্ট ফ্রেমওয়ার্ক কী এবং এটি ডেভেলপারদের কী অর্জন করতে সক্ষম করে?
- দলগুলো কীভাবে দ্রুত প্রোটোটাইপ তৈরি, পুনরাবৃত্তি এবং তাদের এজেন্টের সক্ষমতা উন্নত করতে পারে?
- মাইক্রোসফট দ্বারা তৈরি ফ্রেমওয়ার্ক এবং টুলগুলোর মধ্যে পার্থক্য কী?

, এবং

- আমি কি আমার বিদ্যমান Azure ইকোসিস্টেম টুলগুলো সরাসরি ইন্টিগ্রেট করতে পারি, নাকি আমাকে স্ট্যান্ডঅ্যালোন সমাধান দরকার?
- Azure AI Agents সার্ভিস কী এবং এটি আমাকে কীভাবে সাহায্য করছে?

## শেখার লক্ষ্য

এই পাঠের লক্ষ্য হলো আপনাকে বুঝতে সাহায্য করা:

- এআই এজেন্ট ফ্রেমওয়ার্কের ভূমিকা এআই উন্নয়নে।
- বুদ্ধিমান এজেন্ট তৈরি করতে এআই এজেন্ট ফ্রেমওয়ার্ক ব্যবহার করার উপায়।
- এআই এজেন্ট ফ্রেমওয়ার্ক দ্বারা সক্ষম করা মূল বৈশিষ্ট্য।
- AutoGen, Semantic Kernel এবং Azure AI Agent Service-এর মধ্যে পার্থক্য।

## এআই এজেন্ট ফ্রেমওয়ার্ক কী এবং এটি ডেভেলপারদের কী করতে সক্ষম করে?

প্রথাগত এআই ফ্রেমওয়ার্কগুলো আপনার অ্যাপ্লিকেশনে এআই ইন্টিগ্রেট করতে এবং নিম্নলিখিত উপায়ে এই অ্যাপগুলোকে উন্নত করতে সাহায্য করতে পারে:

- **পার্সোনালাইজেশন**: এআই ব্যবহারকারীর আচরণ এবং পছন্দ বিশ্লেষণ করে ব্যক্তিগতকৃত সুপারিশ, কন্টেন্ট এবং অভিজ্ঞতা প্রদান করতে পারে।
উদাহরণ: Netflix-এর মতো স্ট্রিমিং সার্ভিসগুলো এআই ব্যবহার করে দেখার ইতিহাসের উপর ভিত্তি করে সিনেমা এবং শো সুপারিশ করে, ব্যবহারকারীর সম্পৃক্ততা এবং সন্তুষ্টি বৃদ্ধি করে।
- **স্বয়ংক্রিয়তা এবং দক্ষতা**: এআই পুনরাবৃত্তিমূলক কাজ স্বয়ংক্রিয় করতে, কর্মপ্রবাহ সহজতর করতে এবং অপারেশনাল দক্ষতা উন্নত করতে পারে।
উদাহরণ: কাস্টমার সার্ভিস অ্যাপগুলো এআই-চালিত চ্যাটবট ব্যবহার করে সাধারণ প্রশ্নের উত্তর দেয়, প্রতিক্রিয়া সময় কমায় এবং মানব এজেন্টদের আরও জটিল সমস্যার জন্য মুক্ত করে।
- **উন্নত ব্যবহারকারীর অভিজ্ঞতা**: এআই ভয়েস রিকগনিশন, প্রাকৃতিক ভাষা প্রক্রিয়াকরণ এবং প্রেডিক্টিভ টেক্সটের মতো বুদ্ধিমান বৈশিষ্ট্য প্রদান করে সামগ্রিক ব্যবহারকারীর অভিজ্ঞতা উন্নত করতে পারে।
উদাহরণ: Siri এবং Google Assistant-এর মতো ভার্চুয়াল অ্যাসিস্ট্যান্ট এআই ব্যবহার করে ভয়েস কমান্ড বুঝতে এবং সাড়া দিতে, ব্যবহারকারীদের তাদের ডিভাইসের সাথে যোগাযোগ করা সহজ করে তোলে।

### এটি সবই চমৎকার শোনাচ্ছে, তাই আমরা এআই এজেন্ট ফ্রেমওয়ার্কের প্রয়োজন কেন?

এআই এজেন্ট ফ্রেমওয়ার্কগুলো শুধুমাত্র এআই ফ্রেমওয়ার্কের চেয়ে বেশি কিছু উপস্থাপন করে। এগুলো এমন বুদ্ধিমান এজেন্ট তৈরি করতে ডিজাইন করা হয়েছে যা ব্যবহারকারী, অন্যান্য এজেন্ট এবং পরিবেশের সাথে যোগাযোগ করতে পারে নির্দিষ্ট লক্ষ্য অর্জনের জন্য। এই এজেন্টগুলো স্বায়ত্তশাসিত আচরণ প্রদর্শন করতে পারে, সিদ্ধান্ত নিতে পারে এবং পরিবর্তিত পরিস্থিতির সাথে মানিয়ে নিতে পারে। আসুন এআই এজেন্ট ফ্রেমওয়ার্ক দ্বারা সক্ষম করা কিছু মূল বৈশিষ্ট্য দেখি:

- **এজেন্ট সহযোগিতা এবং সমন্বয়**: একাধিক এআই এজেন্ট তৈরি করা সম্ভব করে যা একসাথে কাজ করতে পারে, যোগাযোগ করতে পারে এবং জটিল কাজ সমাধানে সমন্বয় করতে পারে।
- **কাজের স্বয়ংক্রিয়তা এবং ব্যবস্থাপনা**: মাল্টি-স্টেপ কর্মপ্রবাহ, কাজের প্রতিনিধিত্ব এবং এজেন্টদের মধ্যে গতিশীল কাজ ব্যবস্থাপনার জন্য প্রক্রিয়া প্রদান করে।
- **প্রাসঙ্গিক বোঝা এবং অভিযোজন**: এজেন্টদের প্রাসঙ্গিকতা বুঝতে, পরিবর্তিত পরিবেশের সাথে মানিয়ে নিতে এবং রিয়েল-টাইম তথ্যের উপর ভিত্তি করে সিদ্ধান্ত নিতে সক্ষম করে।

সারসংক্ষেপে, এজেন্টগুলো আপনাকে আরও বেশি কিছু করতে দেয়, স্বয়ংক্রিয়তাকে পরবর্তী স্তরে নিয়ে যায়, আরও বুদ্ধিমান সিস্টেম তৈরি করে যা তাদের পরিবেশ থেকে শিখতে এবং মানিয়ে নিতে পারে।

## কীভাবে দ্রুত প্রোটোটাইপ তৈরি, পুনরাবৃত্তি এবং এজেন্টের সক্ষমতা উন্নত করবেন?

এটি একটি দ্রুত পরিবর্তনশীল ক্ষেত্র, তবে বেশিরভাগ এআই এজেন্ট ফ্রেমওয়ার্কে কিছু সাধারণ বিষয় রয়েছে যা আপনাকে দ্রুত প্রোটোটাইপ এবং পুনরাবৃত্তি করতে সাহায্য করতে পারে, যথা মডিউল কম্পোনেন্ট, সহযোগী টুল এবং রিয়েল-টাইম লার্নিং। আসুন এগুলো নিয়ে আলোচনা করি:

- **মডুলার কম্পোনেন্ট ব্যবহার করুন**: এআই SDK-গুলো প্রি-বিল্ট কম্পোনেন্ট সরবরাহ করে যেমন এআই এবং মেমরি সংযোগকারী, প্রাকৃতিক ভাষা বা কোড প্লাগইন ব্যবহার করে ফাংশন কলিং, প্রম্পট টেমপ্লেট এবং আরও অনেক কিছু।
- **সহযোগী টুল ব্যবহার করুন**: নির্দিষ্ট ভূমিকা এবং কাজের জন্য এজেন্ট ডিজাইন করুন, তাদের সহযোগী কর্মপ্রবাহ পরীক্ষা এবং পরিমার্জন সক্ষম করুন।
- **রিয়েল-টাইমে শিখুন**: প্রতিক্রিয়া লুপ বাস্তবায়ন করুন যেখানে এজেন্টগুলো ইন্টারঅ্যাকশন থেকে শিখে এবং তাদের আচরণ গতিশীলভাবে সামঞ্জস্য করে।

### মডুলার কম্পোনেন্ট ব্যবহার করুন

Microsoft Semantic Kernel এবং LangChain-এর মতো SDK-গুলো প্রি-বিল্ট কম্পোনেন্ট সরবরাহ করে যেমন এআই সংযোগকারী, প্রম্পট টেমপ্লেট এবং মেমরি ব্যবস্থাপনা।

**দলগুলো কীভাবে এগুলো ব্যবহার করতে পারে**: দলগুলো এই কম্পোনেন্টগুলো দ্রুত একত্রিত করে একটি কার্যকরী প্রোটোটাইপ তৈরি করতে পারে, যা স্ক্র্যাচ থেকে শুরু না করেই দ্রুত পরীক্ষা এবং পুনরাবৃত্তি করার অনুমতি দেয়।

**এটি বাস্তবে কীভাবে কাজ করে**: আপনি একটি প্রি-বিল্ট পার্সার ব্যবহার করতে পারেন ব্যবহারকারীর ইনপুট থেকে তথ্য বের করতে, একটি মেমরি মডিউল ডেটা সংরক্ষণ এবং পুনরুদ্ধার করতে এবং একটি প্রম্পট জেনারেটর ব্যবহারকারীদের সাথে যোগাযোগ করতে, সবই স্ক্র্যাচ থেকে এই কম্পোনেন্টগুলো তৈরি না করেই।

**উদাহরণ কোড**। আসুন উদাহরণ দেখি কীভাবে আপনি Semantic Kernel Python এবং .Net-এর সাথে একটি প্রি-বিল্ট এআই সংযোগকারী ব্যবহার করতে পারেন যা অটো-ফাংশন কলিং ব্যবহার করে মডেলকে ব্যবহারকারীর ইনপুটের প্রতিক্রিয়া জানাতে সক্ষম করে:

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

এই উদাহরণ থেকে আপনি দেখতে পাচ্ছেন কীভাবে আপনি একটি প্রি-বিল্ট পার্সার ব্যবহার করে ব্যবহারকারীর ইনপুট থেকে মূল তথ্য বের করতে পারেন, যেমন একটি ফ্লাইট বুকিং অনুরোধের উৎস, গন্তব্য এবং তারিখ। এই মডুলার পদ্ধতি আপনাকে উচ্চ-স্তরের যুক্তির উপর মনোযোগ কেন্দ্রীভূত করতে দেয়।

### সহযোগী টুল ব্যবহার করুন

CrewAI, Microsoft AutoGen এবং Semantic Kernel-এর মতো ফ্রেমওয়ার্কগুলো একাধিক এজেন্ট তৈরি করার সুবিধা দেয় যা একসাথে কাজ করতে পারে।

**দলগুলো কীভাবে এগুলো ব্যবহার করতে পারে**: দলগুলো নির্দিষ্ট ভূমিকা এবং কাজের জন্য এজেন্ট ডিজাইন করতে পারে, তাদের সহযোগী কর্মপ্রবাহ পরীক্ষা এবং পরিমার্জন করতে পারে এবং সামগ্রিক সিস্টেম দক্ষতা উন্নত করতে পারে।

**এটি বাস্তবে কীভাবে কাজ করে**: আপনি এজেন্টদের একটি দল তৈরি করতে পারেন যেখানে প্রতিটি এজেন্টের একটি বিশেষ ফাংশন রয়েছে, যেমন ডেটা পুনরুদ্ধার, বিশ্লেষণ বা সিদ্ধান্ত গ্রহণ। এই এজেন্টগুলো একটি সাধারণ লক্ষ্য অর্জনের জন্য তথ্য যোগাযোগ এবং শেয়ার করতে পারে, যেমন ব্যবহারকারীর প্রশ্নের উত্তর দেওয়া বা একটি কাজ সম্পন্ন করা।

**উদাহরণ কোড (AutoGen)**:

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

পূর্ববর্তী কোডে আপনি দেখতে পাচ্ছেন কীভাবে আপনি একটি কাজ তৈরি করতে পারেন যা একাধিক এজেন্ট একসাথে কাজ করে ডেটা বিশ্লেষণ করতে। প্রতিটি এজেন্ট একটি নির্দিষ্ট ফাংশন সম্পাদন করে, এবং কাজটি এজেন্টদের সমন্বয় করে কাঙ্ক্ষিত ফলাফল অর্জনের মাধ্যমে সম্পন্ন হয়। বিশেষ ভূমিকা সহ নিবেদিত এজেন্ট তৈরি করে, আপনি কাজের দক্ষতা এবং কর্মক্ষমতা উন্নত করতে পারেন।

### রিয়েল-টাইমে শিখুন

উন্নত ফ্রেমওয়ার্কগুলো রিয়েল-টাইম প্রাসঙ্গিক বোঝা এবং অভিযোজনের জন্য সক্ষমতা প্রদান করে।

**দলগুলো কীভাবে এগুলো ব্যবহার করতে পারে**: দলগুলো প্রতিক্রিয়া লুপ বাস্তবায়ন করতে পারে যেখানে এজেন্টগুলো ইন্টারঅ্যাকশন থেকে শিখে এবং তাদের আচরণ গতিশীলভাবে সামঞ্জস্য করে, যার ফলে সক্ষমতার ক্রমাগত উন্নতি এবং পরিমার্জন ঘটে।

**এটি বাস্তবে কীভাবে কাজ করে**: এজেন্টগুলো ব্যবহারকারীর প্রতিক্রিয়া, পরিবেশগত ডেটা এবং কাজের ফলাফল বিশ্লেষণ করতে পারে তাদের জ্ঞানভাণ্ডার আপডেট করতে, সিদ্ধান্ত গ্রহণের অ্যালগরিদম সামঞ্জস্য করতে এবং সময়ের সাথে কর্মক্ষমতা উন্নত করতে। এই পুনরাবৃত্তিমূলক শেখার প্রক্রিয়া এজেন্টগুলোকে পরিবর্তিত পরিস্থিতি এবং ব্যবহারকারীর পছন্দের সাথে মানিয়ে নিতে সক্ষম করে, সামগ্রিক সিস্টেম কার্যকারিতা উন্নত করে।

## AutoGen, Semantic Kernel এবং Azure AI Agent Service-এর মধ্যে পার্থক্য কী?

এই ফ্রেমওয়ার্কগুলো তুলনা করার অনেক উপায় রয়েছে, তবে আসুন তাদের ডিজাইন, সক্ষমতা এবং লক্ষ্য ব্যবহার ক্ষেত্রে কিছু মূল পার্থক্য দেখি:

## AutoGen

AutoGen হলো Microsoft Research-এর AI Frontiers Lab দ্বারা তৈরি একটি ওপেন-সোর্স ফ্রেমওয়ার্ক। এটি ইভেন্ট-চালিত, বিতরণ করা *agentic* অ্যাপ্লিকেশনগুলোর উপর ফোকাস করে, একাধিক LLMs এবং SLMs, টুল এবং উন্নত মাল্টি-এজেন্ট ডিজাইন প্যাটার্ন সক্ষম করে।

AutoGen এজেন্টের মূল ধারণার উপর ভিত্তি করে তৈরি করা হয়েছে, যা স্বায়ত্তশাসিত সত্তা যা তাদের পরিবেশ উপলব্ধি করতে পারে, সিদ্ধান্ত নিতে পারে এবং নির্দিষ্ট লক্ষ্য অর্জনের জন্য পদক্ষেপ নিতে পারে। এজেন্টগুলো অ্যাসিঙ্ক্রোনাস মেসেজের মাধ্যমে যোগাযোগ করে, তাদের স্বাধীনভাবে এবং সমান্তরালভাবে কাজ করার অনুমতি দেয়, সিস্টেমের স্কেলেবিলিটি এবং প্রতিক্রিয়াশীলতা বৃদ্ধি করে।
## এজেন্ট ফ্রেমওয়ার্ক সম্পর্কে কী?

## Azure AI Agent Service

Azure AI Agent Service হলো একটি নতুন সংযোজন, যা Microsoft Ignite 2024-এ পরিচিত হয়। এটি আরও নমনীয় মডেলের সাথে AI এজেন্ট তৈরি এবং স্থাপন করার সুযোগ দেয়, যেমন সরাসরি ওপেন-সোর্স LLMs (যেমন Llama 3, Mistral, এবং Cohere) কল করা।

Azure AI Agent Service শক্তিশালী এন্টারপ্রাইজ নিরাপত্তা ব্যবস্থা এবং ডেটা সংরক্ষণ পদ্ধতি প্রদান করে, যা এটিকে এন্টারপ্রাইজ অ্যাপ্লিকেশনের জন্য উপযুক্ত করে তোলে।

এটি AutoGen এবং Semantic Kernel-এর মতো মাল্টি-এজেন্ট অর্কেস্ট্রেশন ফ্রেমওয়ার্কের সাথে সরাসরি কাজ করে।

এই পরিষেবা বর্তমানে পাবলিক প্রিভিউতে রয়েছে এবং এজেন্ট তৈরির জন্য Python এবং C# সমর্থন করে।

Semantic Kernel Python ব্যবহার করে, আমরা একটি ব্যবহারকারী-সংজ্ঞায়িত প্লাগইনের মাধ্যমে একটি Azure AI Agent তৈরি করতে পারি:

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

### মূল ধারণা

Azure AI Agent Service-এর নিম্নলিখিত মূল ধারণাগুলি রয়েছে:

- **Agent**। Azure AI Agent Service, Azure AI Foundry-এর সাথে সংযুক্ত। AI Foundry-তে, একটি AI Agent একটি "স্মার্ট" মাইক্রোসার্ভিস হিসেবে কাজ করে যা প্রশ্নের উত্তর দিতে (RAG), কাজ সম্পাদন করতে, বা সম্পূর্ণ ওয়ার্কফ্লো স্বয়ংক্রিয় করতে ব্যবহৃত হয়। এটি জেনারেটিভ AI মডেলের শক্তি এবং বাস্তব-জগতের ডেটা সোর্সের সাথে ইন্টারঅ্যাক্ট করার সরঞ্জামগুলির সংমিশ্রণে এটি অর্জন করে। একটি এজেন্টের উদাহরণ এখানে দেওয়া হলো:

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    এই উদাহরণে, একটি এজেন্ট তৈরি করা হয়েছে মডেল `gpt-4o-mini`, নাম `my-agent`, এবং নির্দেশনা `You are helpful agent` দিয়ে। এজেন্টটি কোড ইন্টারপ্রিটেশন কাজ সম্পাদনের জন্য সরঞ্জাম এবং সম্পদ দিয়ে সজ্জিত।

- **Thread এবং Messages**। থ্রেড আরেকটি গুরুত্বপূর্ণ ধারণা। এটি একটি এজেন্ট এবং ব্যবহারকারীর মধ্যে কথোপকথন বা ইন্টারঅ্যাকশনের প্রতিনিধিত্ব করে। থ্রেডগুলি কথোপকথনের অগ্রগতি ট্র্যাক করতে, প্রসঙ্গ তথ্য সংরক্ষণ করতে এবং ইন্টারঅ্যাকশনের অবস্থা পরিচালনা করতে ব্যবহৃত হয়। একটি থ্রেডের উদাহরণ এখানে দেওয়া হলো:

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

    পূর্ববর্তী কোডে, একটি থ্রেড তৈরি করা হয়েছে। এরপর, থ্রেডে একটি বার্তা পাঠানো হয়েছে। `create_and_process_run` কল করে, এজেন্টকে থ্রেডে কাজ সম্পাদন করতে বলা হয়েছে। অবশেষে, বার্তাগুলি সংগ্রহ করা হয়েছে এবং এজেন্টের প্রতিক্রিয়া দেখতে লগ করা হয়েছে। বার্তাগুলি ব্যবহারকারী এবং এজেন্টের মধ্যে কথোপকথনের অগ্রগতি নির্দেশ করে। এটি বোঝা গুরুত্বপূর্ণ যে বার্তাগুলি বিভিন্ন ধরণের হতে পারে যেমন টেক্সট, ইমেজ, বা ফাইল, যা এজেন্টের কাজের ফলাফল হতে পারে। একজন ডেভেলপার হিসেবে, আপনি এই তথ্যটি ব্যবহার করে প্রতিক্রিয়াটি আরও প্রক্রিয়াকরণ করতে বা ব্যবহারকারীর কাছে উপস্থাপন করতে পারেন।

- **অন্যান্য AI ফ্রেমওয়ার্কের সাথে সংযুক্তি**। Azure AI Agent Service অন্যান্য ফ্রেমওয়ার্ক যেমন AutoGen এবং Semantic Kernel-এর সাথে ইন্টারঅ্যাক্ট করতে পারে, যার মানে আপনি আপনার অ্যাপ্লিকেশনের একটি অংশ এই ফ্রেমওয়ার্কগুলির একটিতে তৈরি করতে পারেন এবং উদাহরণস্বরূপ এজেন্ট সার্ভিসকে অর্কেস্ট্রেটর হিসেবে ব্যবহার করতে পারেন অথবা সবকিছু এজেন্ট সার্ভিসে তৈরি করতে পারেন।

**ব্যবহার ক্ষেত্র**: Azure AI Agent Service এন্টারপ্রাইজ অ্যাপ্লিকেশনের জন্য ডিজাইন করা হয়েছে যা নিরাপদ, স্কেলযোগ্য এবং নমনীয় AI এজেন্ট স্থাপনের প্রয়োজন।

## এই ফ্রেমওয়ার্কগুলির মধ্যে পার্থক্য কী?

এটি মনে হতে পারে যে এই ফ্রেমওয়ার্কগুলির মধ্যে অনেক ওভারল্যাপ রয়েছে, তবে তাদের নকশা, ক্ষমতা এবং লক্ষ্য ব্যবহার ক্ষেত্রে কিছু মূল পার্থক্য রয়েছে:

- **AutoGen**: এটি মাল্টি-এজেন্ট সিস্টেমের উপর গবেষণার জন্য একটি পরীক্ষামূলক ফ্রেমওয়ার্ক। এটি জটিল মাল্টি-এজেন্ট সিস্টেম পরীক্ষা এবং প্রোটোটাইপ করার জন্য সেরা জায়গা।
- **Semantic Kernel**: এটি এন্টারপ্রাইজ এজেন্টিক অ্যাপ্লিকেশন তৈরির জন্য একটি প্রোডাকশন-রেডি এজেন্ট লাইব্রেরি। এটি ইভেন্ট-চালিত, বিতরণকৃত এজেন্টিক অ্যাপ্লিকেশনগুলিতে ফোকাস করে, যা একাধিক LLMs এবং SLMs, সরঞ্জাম এবং একক/মাল্টি-এজেন্ট ডিজাইন প্যাটার্ন সক্ষম করে।
- **Azure AI Agent Service**: এটি Azure Foundry-তে এজেন্টের জন্য একটি প্ল্যাটফর্ম এবং স্থাপন পরিষেবা। এটি Azure OpenAI, Azure AI Search, Bing Search এবং কোড এক্সিকিউশনের মতো পরিষেবাগুলির সাথে সংযোগ তৈরি করার ক্ষমতা প্রদান করে।

এখনও নিশ্চিত নন কোনটি বেছে নেবেন?

### ব্যবহার ক্ষেত্র

আসুন কিছু সাধারণ ব্যবহার ক্ষেত্রের মাধ্যমে আপনাকে সাহায্য করার চেষ্টা করি:

> প্রশ্ন: আমি পরীক্ষা করছি, শিখছি এবং প্রুফ-অফ-কনসেপ্ট এজেন্ট অ্যাপ্লিকেশন তৈরি করছি, এবং আমি দ্রুত তৈরি এবং পরীক্ষা করতে চাই।
>
> উত্তর: এই পরিস্থিতির জন্য AutoGen একটি ভালো পছন্দ হবে, কারণ এটি ইভেন্ট-চালিত, বিতরণকৃত এজেন্টিক অ্যাপ্লিকেশনগুলিতে ফোকাস করে এবং উন্নত মাল্টি-এজেন্ট ডিজাইন প্যাটার্ন সমর্থন করে।

> প্রশ্ন: এই ক্ষেত্রে Semantic Kernel এবং Azure AI Agent Service-এর চেয়ে AutoGen কেন ভালো পছন্দ?
>
> উত্তর: AutoGen বিশেষভাবে ইভেন্ট-চালিত, বিতরণকৃত এজেন্টিক অ্যাপ্লিকেশনগুলির জন্য ডিজাইন করা হয়েছে, যা এটিকে কোড জেনারেশন এবং ডেটা বিশ্লেষণ কাজ স্বয়ংক্রিয় করার জন্য উপযুক্ত করে তোলে। এটি জটিল মাল্টি-এজেন্ট সিস্টেম দক্ষতার সাথে তৈরি করার জন্য প্রয়োজনীয় সরঞ্জাম এবং ক্ষমতা প্রদান করে।

> প্রশ্ন: মনে হচ্ছে Azure AI Agent Service এখানে কাজ করতে পারে, এটি কোড জেনারেশন এবং আরও অনেক কিছুর জন্য সরঞ্জাম সরবরাহ করে?
>
> উত্তর: হ্যাঁ, Azure AI Agent Service এজেন্টের জন্য একটি প্ল্যাটফর্ম পরিষেবা এবং এতে একাধিক মডেল, Azure AI Search, Bing Search এবং Azure Functions-এর জন্য বিল্ট-ইন ক্ষমতা রয়েছে। এটি Foundry Portal-এ আপনার এজেন্ট তৈরি করা এবং স্কেলে স্থাপন করা সহজ করে তোলে।

> প্রশ্ন: আমি এখনও বিভ্রান্ত, আমাকে একটি বিকল্প দিন।
>
> উত্তর: একটি দুর্দান্ত পছন্দ হলো আপনার অ্যাপ্লিকেশনটি প্রথমে Semantic Kernel-এ তৈরি করা এবং তারপর Azure AI Agent Service ব্যবহার করে আপনার এজেন্ট স্থাপন করা। এই পদ্ধতিটি আপনাকে সহজেই আপনার এজেন্টগুলি সংরক্ষণ করতে দেয় এবং Semantic Kernel-এ মাল্টি-এজেন্ট সিস্টেম তৈরি করার ক্ষমতা ব্যবহার করতে দেয়। এছাড়াও, Semantic Kernel-এ AutoGen-এর একটি সংযোগকারী রয়েছে, যা উভয় ফ্রেমওয়ার্ক একসাথে ব্যবহার করা সহজ করে তোলে।

আসুন একটি টেবিলে মূল পার্থক্যগুলি সংক্ষেপ করি:

| ফ্রেমওয়ার্ক | ফোকাস | মূল ধারণা | ব্যবহার ক্ষেত্র |
| --- | --- | --- | --- |
| AutoGen | ইভেন্ট-চালিত, বিতরণকৃত এজেন্টিক অ্যাপ্লিকেশন | এজেন্ট, পারসোনা, ফাংশন, ডেটা | কোড জেনারেশন, ডেটা বিশ্লেষণ কাজ |
| Semantic Kernel | মানবসদৃশ টেক্সট বিষয়বস্তু বোঝা এবং তৈরি করা | এজেন্ট, মডুলার কম্পোনেন্ট, সহযোগিতা | প্রাকৃতিক ভাষা বোঝা, বিষয়বস্তু তৈরি |
| Azure AI Agent Service | নমনীয় মডেল, এন্টারপ্রাইজ নিরাপত্তা, কোড জেনারেশন, টুল কলিং | মডুলারিটি, সহযোগিতা, প্রক্রিয়া অর্কেস্ট্রেশন | নিরাপদ, স্কেলযোগ্য এবং নমনীয় AI এজেন্ট স্থাপন |

প্রতিটি ফ্রেমওয়ার্কের জন্য আদর্শ ব্যবহার ক্ষেত্র কী?

## আমি কি আমার বিদ্যমান Azure ইকোসিস্টেম টুলগুলি সরাসরি সংযুক্ত করতে পারি, নাকি আমাকে স্ট্যান্ডঅ্যালোন সমাধান প্রয়োজন?

উত্তর হলো হ্যাঁ, আপনি আপনার বিদ্যমান Azure ইকোসিস্টেম টুলগুলি সরাসরি Azure AI Agent Service-এর সাথে সংযুক্ত করতে পারেন, বিশেষত কারণ এটি অন্যান্য Azure পরিষেবাগুলির সাথে নির্বিঘ্নে কাজ করার জন্য তৈরি করা হয়েছে। উদাহরণস্বরূপ, আপনি Bing, Azure AI Search এবং Azure Functions সংযুক্ত করতে পারেন। Azure AI Foundry-এর সাথে গভীর সংযোগও রয়েছে।

AutoGen এবং Semantic Kernel-এর জন্য, আপনি Azure পরিষেবাগুলির সাথে সংযুক্ত করতে পারেন, তবে এটি আপনার কোড থেকে Azure পরিষেবাগুলি কল করার প্রয়োজন হতে পারে। আরেকটি উপায় হলো Azure SDKs ব্যবহার করে আপনার এজেন্ট থেকে Azure পরিষেবাগুলির সাথে ইন্টারঅ্যাক্ট করা। এছাড়াও, যেমন উল্লেখ করা হয়েছে, আপনি AutoGen বা Semantic Kernel-এ তৈরি এজেন্টগুলির জন্য অর্কেস্ট্রেটর হিসাবে Azure AI Agent Service ব্যবহার করতে পারেন, যা Azure ইকোসিস্টেমে সহজ অ্যাক্সেস প্রদান করবে।

### AI এজেন্ট ফ্রেমওয়ার্ক সম্পর্কে আরও প্রশ্ন আছে?

[Azure AI Foundry Discord](https://aka.ms/ai-agents/discord)-এ যোগ দিন, অন্যান্য শিক্ষার্থীদের সাথে দেখা করুন, অফিস আওয়ার্সে অংশ নিন এবং আপনার AI এজেন্ট সম্পর্কিত প্রশ্নগুলির উত্তর পান।

## রেফারেন্স

- 

## পূর্ববর্তী পাঠ

[AI এজেন্ট এবং এজেন্ট ব্যবহার ক্ষেত্রের পরিচিতি](../01-intro-to-ai-agents/README.md)

## পরবর্তী পাঠ

[এজেন্টিক ডিজাইন প্যাটার্ন বোঝা](../03-agentic-design-patterns/README.md)

---

**অস্বীকৃতি**:  
এই নথিটি AI অনুবাদ পরিষেবা [Co-op Translator](https://github.com/Azure/co-op-translator) ব্যবহার করে অনুবাদ করা হয়েছে। আমরা যথাসম্ভব সঠিক অনুবাদের চেষ্টা করি, তবে অনুগ্রহ করে মনে রাখবেন যে স্বয়ংক্রিয় অনুবাদে ত্রুটি বা অসংগতি থাকতে পারে। নথিটির মূল ভাষায় থাকা সংস্করণটিকেই প্রামাণিক উৎস হিসেবে বিবেচনা করা উচিত। গুরুত্বপূর্ণ তথ্যের জন্য, পেশাদার মানব অনুবাদ ব্যবহার করার পরামর্শ দেওয়া হচ্ছে। এই অনুবাদ ব্যবহারের ফলে সৃষ্ট কোনো ভুল বোঝাবুঝি বা ভুল ব্যাখ্যার জন্য আমরা দায়ী নই।