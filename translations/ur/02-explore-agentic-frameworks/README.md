<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-29T09:35:43+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "ur"
}
-->
[![Exploring AI Agent Frameworks](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.ur.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(اوپر دی گئی تصویر پر کلک کریں تاکہ اس سبق کی ویڈیو دیکھی جا سکے)_

# AI ایجنٹ فریم ورک کا جائزہ لیں

AI ایجنٹ فریم ورک ایسے سافٹ ویئر پلیٹ فارمز ہیں جو AI ایجنٹس کی تخلیق، تعیناتی، اور انتظام کو آسان بناتے ہیں۔ یہ فریم ورک ڈویلپرز کو پہلے سے تیار شدہ اجزاء، خلاصے، اور اوزار فراہم کرتے ہیں جو پیچیدہ AI سسٹمز کی ترقی کو آسان بناتے ہیں۔

یہ فریم ورک ڈویلپرز کو ان کے ایپلیکیشنز کے منفرد پہلوؤں پر توجہ مرکوز کرنے میں مدد دیتے ہیں، AI ایجنٹ کی ترقی میں عام چیلنجز کے لیے معیاری طریقے فراہم کرتے ہیں۔ یہ AI سسٹمز کی توسیع پذیری، رسائی، اور کارکردگی کو بڑھاتے ہیں۔

## تعارف

اس سبق میں شامل ہوگا:

- AI ایجنٹ فریم ورک کیا ہیں اور یہ ڈویلپرز کو کیا حاصل کرنے کے قابل بناتے ہیں؟
- ٹیمیں ان کا استعمال کیسے کر سکتی ہیں تاکہ جلدی پروٹوٹائپ، تکرار، اور اپنے ایجنٹ کی صلاحیتوں کو بہتر بنا سکیں؟
- مائیکروسافٹ کے بنائے گئے فریم ورک اور ٹولز میں کیا فرق ہے؟
- کیا میں اپنے موجودہ Azure ایکوسسٹم ٹولز کو براہ راست ضم کر سکتا ہوں، یا مجھے علیحدہ حل کی ضرورت ہوگی؟
- Azure AI ایجنٹس سروس کیا ہے اور یہ میرے لیے کیسے مددگار ہے؟

## سیکھنے کے مقاصد

اس سبق کے مقاصد یہ ہیں کہ آپ کو سمجھنے میں مدد دی جائے:

- AI ایجنٹ فریم ورک کا AI ترقی میں کردار۔
- AI ایجنٹ فریم ورک کا استعمال کرتے ہوئے ذہین ایجنٹس کیسے بنائیں۔
- AI ایجنٹ فریم ورک کے ذریعے فعال کردہ کلیدی صلاحیتیں۔
- AutoGen، Semantic Kernel، اور Azure AI ایجنٹ سروس کے درمیان فرق۔

## AI ایجنٹ فریم ورک کیا ہیں اور یہ ڈویلپرز کو کیا کرنے کے قابل بناتے ہیں؟

روایتی AI فریم ورک آپ کو اپنے ایپس میں AI کو ضم کرنے اور ان ایپس کو درج ذیل طریقوں سے بہتر بنانے میں مدد دے سکتے ہیں:

- **ذاتی نوعیت**: AI صارف کے رویے اور ترجیحات کا تجزیہ کر کے ذاتی نوعیت کی تجاویز، مواد، اور تجربات فراہم کر سکتا ہے۔
مثال: Netflix جیسی اسٹریمنگ سروسز AI کا استعمال کرتی ہیں تاکہ دیکھنے کی تاریخ کی بنیاد پر فلمیں اور شوز تجویز کیے جا سکیں، جس سے صارف کی مشغولیت اور اطمینان میں اضافہ ہوتا ہے۔
- **خودکاریت اور کارکردگی**: AI بار بار کیے جانے والے کاموں کو خودکار بنا سکتا ہے، ورک فلو کو ہموار کر سکتا ہے، اور آپریشنل کارکردگی کو بہتر بنا سکتا ہے۔
مثال: کسٹمر سروس ایپس AI سے چلنے والے چیٹ بوٹس کا استعمال کرتی ہیں تاکہ عام سوالات کو سنبھالا جا سکے، جواب کے وقت کو کم کیا جا سکے اور انسانی ایجنٹس کو زیادہ پیچیدہ مسائل کے لیے آزاد کیا جا سکے۔
- **بہتر صارف تجربہ**: AI ذہین خصوصیات جیسے کہ آواز کی پہچان، قدرتی زبان کی پروسیسنگ، اور پیش گوئی کرنے والے متن فراہم کر کے مجموعی صارف کے تجربے کو بہتر بنا سکتا ہے۔
مثال: Siri اور Google Assistant جیسے ورچوئل اسسٹنٹس AI کا استعمال کرتے ہیں تاکہ آواز کے احکامات کو سمجھا جا سکے اور ان کا جواب دیا جا سکے، جس سے صارفین کے لیے اپنے آلات کے ساتھ تعامل کرنا آسان ہو جاتا ہے۔

### یہ سب بہت اچھا لگتا ہے، تو پھر ہمیں AI ایجنٹ فریم ورک کی ضرورت کیوں ہے؟

AI ایجنٹ فریم ورک صرف AI فریم ورک سے زیادہ کی نمائندگی کرتے ہیں۔ یہ ذہین ایجنٹس کی تخلیق کو فعال کرنے کے لیے ڈیزائن کیے گئے ہیں جو صارفین، دیگر ایجنٹس، اور ماحول کے ساتھ تعامل کر سکتے ہیں تاکہ مخصوص اہداف حاصل کیے جا سکیں۔ یہ ایجنٹس خود مختار رویہ ظاہر کر سکتے ہیں، فیصلے کر سکتے ہیں، اور بدلتے ہوئے حالات کے مطابق ڈھال سکتے ہیں۔ آئیے AI ایجنٹ فریم ورک کے ذریعے فعال کردہ کچھ کلیدی صلاحیتوں پر نظر ڈالیں:

- **ایجنٹ تعاون اور ہم آہنگی**: متعدد AI ایجنٹس کی تخلیق کو فعال کریں جو مل کر کام کر سکیں، بات چیت کر سکیں، اور پیچیدہ کاموں کو حل کرنے کے لیے ہم آہنگی کر سکیں۔
- **کام کی خودکاریت اور انتظام**: ملٹی اسٹیپ ورک فلو، کام کی تفویض، اور ایجنٹس کے درمیان متحرک کام کے انتظام کے لیے میکانزم فراہم کریں۔
- **سیاق و سباق کی تفہیم اور موافقت**: ایجنٹس کو سیاق و سباق کو سمجھنے، بدلتے ہوئے ماحول کے مطابق ڈھالنے، اور حقیقی وقت کی معلومات کی بنیاد پر فیصلے کرنے کی صلاحیت سے آراستہ کریں۔

خلاصہ یہ کہ ایجنٹس آپ کو مزید کرنے کی اجازت دیتے ہیں، خودکاریت کو اگلے درجے تک لے جاتے ہیں، اور زیادہ ذہین سسٹمز تخلیق کرتے ہیں جو اپنے ماحول سے سیکھ سکتے ہیں اور اس کے مطابق ڈھال سکتے ہیں۔

## ایجنٹ کی صلاحیتوں کو جلدی پروٹوٹائپ، تکرار، اور بہتر کیسے کریں؟

یہ ایک تیزی سے بدلتا ہوا منظرنامہ ہے، لیکن AI ایجنٹ فریم ورک میں کچھ چیزیں عام ہیں جو آپ کو جلدی پروٹوٹائپ اور تکرار کرنے میں مدد دے سکتی ہیں، جیسے ماڈیولر اجزاء، تعاون کے اوزار، اور حقیقی وقت میں سیکھنا۔ آئیے ان پر تفصیل سے بات کریں:

- **ماڈیولر اجزاء کا استعمال کریں**: AI SDKs پہلے سے تیار شدہ اجزاء پیش کرتے ہیں جیسے AI اور میموری کنیکٹرز، قدرتی زبان یا کوڈ پلگ انز کا استعمال کرتے ہوئے فنکشن کالنگ، پرامپٹ ٹیمپلیٹس، اور مزید۔
- **تعاون کے اوزار استعمال کریں**: ایجنٹس کو مخصوص کرداروں اور کاموں کے ساتھ ڈیزائن کریں، جس سے وہ تعاون کے ورک فلو کو جانچنے اور بہتر بنانے کے قابل ہوں۔
- **حقیقی وقت میں سیکھیں**: فیڈ بیک لوپس کو نافذ کریں جہاں ایجنٹس تعاملات سے سیکھیں اور اپنے رویے کو متحرک طور پر ایڈجسٹ کریں۔

### ماڈیولر اجزاء کا استعمال کریں

Microsoft Semantic Kernel اور LangChain جیسے SDKs پہلے سے تیار شدہ اجزاء پیش کرتے ہیں جیسے AI کنیکٹرز، پرامپٹ ٹیمپلیٹس، اور میموری مینجمنٹ۔

**ٹیمیں ان کا استعمال کیسے کر سکتی ہیں**: ٹیمیں ان اجزاء کو جلدی سے جمع کر کے ایک فعال پروٹوٹائپ بنا سکتی ہیں، بغیر شروع سے شروع کیے، جس سے تیزی سے تجربہ کرنے اور تکرار کرنے کی اجازت ملتی ہے۔

**یہ عملی طور پر کیسے کام کرتا ہے**: آپ صارف کے ان پٹ سے معلومات نکالنے کے لیے پہلے سے تیار شدہ پارسر، ڈیٹا کو ذخیرہ کرنے اور بازیافت کرنے کے لیے میموری ماڈیول، اور صارفین کے ساتھ تعامل کے لیے پرامپٹ جنریٹر استعمال کر سکتے ہیں، یہ سب کچھ ان اجزاء کو شروع سے بنانے کے بغیر۔

**مثال کوڈ**۔ آئیے دیکھتے ہیں کہ آپ Semantic Kernel Python اور .Net کے ساتھ پہلے سے تیار شدہ AI کنیکٹر کا استعمال کرتے ہوئے ماڈل کو صارف کے ان پٹ کا جواب دینے کے لیے کیسے استعمال کر سکتے ہیں:

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

اس مثال سے آپ دیکھ سکتے ہیں کہ آپ صارف کے ان پٹ سے کلیدی معلومات نکالنے کے لیے پہلے سے تیار شدہ پارسر کا فائدہ کیسے اٹھا سکتے ہیں، جیسے کہ فلائٹ بکنگ درخواست کے اصل، منزل، اور تاریخ۔ یہ ماڈیولر نقطہ نظر آپ کو اعلی سطحی منطق پر توجہ مرکوز کرنے کی اجازت دیتا ہے۔

### تعاون کے اوزار استعمال کریں

CrewAI، Microsoft AutoGen، اور Semantic Kernel جیسے فریم ورک متعدد ایجنٹس کی تخلیق کو آسان بناتے ہیں جو مل کر کام کر سکتے ہیں۔

**ٹیمیں ان کا استعمال کیسے کر سکتی ہیں**: ٹیمیں مخصوص کرداروں اور کاموں کے ساتھ ایجنٹس کو ڈیزائن کر سکتی ہیں، جس سے وہ تعاون کے ورک فلو کو جانچنے اور بہتر بنانے اور مجموعی نظام کی کارکردگی کو بہتر بنانے کے قابل ہو سکتی ہیں۔

**یہ عملی طور پر کیسے کام کرتا ہے**: آپ ایجنٹس کی ایک ٹیم بنا سکتے ہیں جہاں ہر ایجنٹ کے پاس ایک مخصوص فنکشن ہوتا ہے، جیسے ڈیٹا بازیافت، تجزیہ، یا فیصلہ سازی۔ یہ ایجنٹس معلومات کا اشتراک اور بات چیت کر سکتے ہیں تاکہ ایک مشترکہ مقصد حاصل کیا جا سکے، جیسے کہ صارف کے سوال کا جواب دینا یا کوئی کام مکمل کرنا۔

**مثال کوڈ (AutoGen)**:

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

پچھلے کوڈ میں آپ دیکھ سکتے ہیں کہ آپ ایک ایسا کام کیسے بنا سکتے ہیں جس میں متعدد ایجنٹس ڈیٹا کا تجزیہ کرنے کے لیے مل کر کام کرتے ہیں۔ ہر ایجنٹ ایک مخصوص فنکشن انجام دیتا ہے، اور کام کو مطلوبہ نتیجہ حاصل کرنے کے لیے ایجنٹس کو مربوط کر کے انجام دیا جاتا ہے۔ مخصوص کرداروں کے ساتھ وقف شدہ ایجنٹس بنا کر، آپ کام کی کارکردگی اور کارکردگی کو بہتر بنا سکتے ہیں۔

### حقیقی وقت میں سیکھیں

جدید فریم ورک حقیقی وقت کے سیاق و سباق کی تفہیم اور موافقت کے لیے صلاحیتیں فراہم کرتے ہیں۔

**ٹیمیں ان کا استعمال کیسے کر سکتی ہیں**: ٹیمیں فیڈ بیک لوپس کو نافذ کر سکتی ہیں جہاں ایجنٹس تعاملات سے سیکھیں اور اپنے رویے کو متحرک طور پر ایڈجسٹ کریں، جس سے صلاحیتوں کی مسلسل بہتری اور بہتری ممکن ہو۔

**یہ عملی طور پر کیسے کام کرتا ہے**: ایجنٹس صارف کے فیڈ بیک، ماحولیاتی ڈیٹا، اور کام کے نتائج کا تجزیہ کر کے اپنے علم کے ذخیرے کو اپ ڈیٹ کر سکتے ہیں، فیصلہ سازی کے الگورتھمز کو ایڈجسٹ کر سکتے ہیں، اور وقت کے ساتھ کارکردگی کو بہتر بنا سکتے ہیں۔ یہ تکراری سیکھنے کا عمل ایجنٹس کو بدلتے ہوئے حالات اور صارف کی ترجیحات کے مطابق ڈھالنے کے قابل بناتا ہے، جس سے مجموعی نظام کی تاثیر میں اضافہ ہوتا ہے۔

## AutoGen، Semantic Kernel اور Azure AI ایجنٹ سروس کے درمیان کیا فرق ہے؟

ان فریم ورک کا موازنہ کرنے کے کئی طریقے ہیں، لیکن آئیے ان کے ڈیزائن، صلاحیتوں، اور ہدف کے استعمال کے معاملات کے لحاظ سے کچھ اہم فرق دیکھتے ہیں:

## AutoGen

AutoGen ایک اوپن سورس فریم ورک ہے جو Microsoft Research کے AI Frontiers Lab نے تیار کیا ہے۔ یہ ایونٹ ڈرائیو، تقسیم شدہ *ایجنٹک* ایپلیکیشنز پر توجہ مرکوز کرتا ہے، جو متعدد LLMs اور SLMs، ٹولز، اور جدید ملٹی ایجنٹ ڈیزائن پیٹرنز کو فعال کرتا ہے۔

AutoGen ایجنٹس کے بنیادی تصور کے ارد گرد بنایا گیا ہے، جو خود مختار ادارے ہیں جو اپنے ماحول کو سمجھ سکتے ہیں، فیصلے کر سکتے ہیں، اور مخصوص اہداف حاصل کرنے کے لیے اقدامات کر سکتے ہیں۔ ایجنٹس غیر متزامن پیغامات کے ذریعے بات چیت کرتے ہیں، جو انہیں آزادانہ اور متوازی طور پر کام کرنے کی اجازت دیتا ہے، جس سے نظام کی توسیع پذیری اور ردعمل میں اضافہ ہوتا ہے۔
تو یہ تھا Semantic Kernel فریم ورک کا بنیادی تعارف، اب بات کرتے ہیں Agent Framework کی۔

## Azure AI Agent Service

Azure AI Agent Service ایک حالیہ اضافہ ہے، جو Microsoft Ignite 2024 میں متعارف کرایا گیا۔ یہ زیادہ لچکدار ماڈلز کے ساتھ AI ایجنٹس کی ترقی اور تعیناتی کی اجازت دیتا ہے، جیسے کہ اوپن سورس LLMs جیسے Llama 3، Mistral، اور Cohere کو براہ راست کال کرنا۔

Azure AI Agent Service مضبوط انٹرپرائز سیکیورٹی میکانزم اور ڈیٹا اسٹوریج کے طریقے فراہم کرتا ہے، جو اسے انٹرپرائز ایپلیکیشنز کے لیے موزوں بناتا ہے۔

یہ سروس AutoGen اور Semantic Kernel جیسے ملٹی ایجنٹ آرکیسٹریشن فریم ورکس کے ساتھ فوری طور پر کام کرتی ہے۔

یہ سروس اس وقت Public Preview میں ہے اور ایجنٹس بنانے کے لیے Python اور C# کو سپورٹ کرتی ہے۔

Semantic Kernel Python کا استعمال کرتے ہوئے، ہم ایک یوزر ڈیفائنڈ پلگ ان کے ساتھ Azure AI Agent بنا سکتے ہیں:

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

### بنیادی تصورات

Azure AI Agent Service کے درج ذیل بنیادی تصورات ہیں:

- **Agent**۔ Azure AI Agent Service، Azure AI Foundry کے ساتھ انٹیگریٹ کرتا ہے۔ AI Foundry کے اندر، ایک AI Agent ایک "سمارٹ" مائیکروسروس کے طور پر کام کرتا ہے جو سوالات کے جوابات دینے (RAG)، اعمال انجام دینے، یا ورک فلو کو مکمل طور پر خودکار کرنے کے لیے استعمال کیا جا سکتا ہے۔ یہ جنریٹو AI ماڈلز کی طاقت کو ان ٹولز کے ساتھ جوڑ کر حاصل کرتا ہے جو اسے حقیقی دنیا کے ڈیٹا ذرائع تک رسائی اور تعامل کی اجازت دیتے ہیں۔ یہاں ایک ایجنٹ کی مثال ہے:

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    اس مثال میں، ایک ایجنٹ `gpt-4o-mini` ماڈل، `my-agent` نام، اور `You are helpful agent` ہدایات کے ساتھ بنایا گیا ہے۔ ایجنٹ کو کوڈ انٹرپریٹیشن کے کام انجام دینے کے لیے ٹولز اور وسائل سے لیس کیا گیا ہے۔

- **Thread اور Messages**۔ تھریڈ ایک اور اہم تصور ہے۔ یہ ایجنٹ اور یوزر کے درمیان گفتگو یا تعامل کی نمائندگی کرتا ہے۔ تھریڈز کو گفتگو کی پیش رفت کو ٹریک کرنے، سیاق و سباق کی معلومات کو ذخیرہ کرنے، اور تعامل کی حالت کو منظم کرنے کے لیے استعمال کیا جا سکتا ہے۔ یہاں ایک تھریڈ کی مثال ہے:

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

    پچھلے کوڈ میں، ایک تھریڈ بنایا گیا ہے۔ اس کے بعد، تھریڈ کو ایک میسج بھیجا جاتا ہے۔ `create_and_process_run` کو کال کرکے، ایجنٹ سے کہا جاتا ہے کہ وہ تھریڈ پر کام کرے۔ آخر میں، میسجز کو ایجنٹ کے جواب کو دیکھنے کے لیے لاگ کیا جاتا ہے۔ میسجز یوزر اور ایجنٹ کے درمیان گفتگو کی پیش رفت کی نشاندہی کرتے ہیں۔ یہ سمجھنا بھی ضروری ہے کہ میسجز مختلف اقسام کے ہو سکتے ہیں جیسے کہ ٹیکسٹ، امیج، یا فائل، جو ایجنٹ کے کام کا نتیجہ ہو سکتے ہیں، مثلاً ایک امیج یا ٹیکسٹ جواب۔ ایک ڈویلپر کے طور پر، آپ اس معلومات کو مزید جواب کو پروسیس کرنے یا یوزر کو پیش کرنے کے لیے استعمال کر سکتے ہیں۔

- **دیگر AI فریم ورکس کے ساتھ انٹیگریشن**۔ Azure AI Agent Service دیگر فریم ورکس جیسے AutoGen اور Semantic Kernel کے ساتھ تعامل کر سکتا ہے، جس کا مطلب ہے کہ آپ اپنی ایپ کا کچھ حصہ ان فریم ورکس میں بنا سکتے ہیں اور مثال کے طور پر ایجنٹ سروس کو آرکیسٹریٹر کے طور پر استعمال کر سکتے ہیں یا آپ سب کچھ ایجنٹ سروس میں بنا سکتے ہیں۔

**استعمال کے کیسز**: Azure AI Agent Service انٹرپرائز ایپلیکیشنز کے لیے ڈیزائن کیا گیا ہے جو محفوظ، اسکیل ایبل، اور لچکدار AI ایجنٹ کی تعیناتی کی ضرورت رکھتے ہیں۔

## ان فریم ورکس میں کیا فرق ہے؟

یہ سننے میں آتا ہے کہ ان فریم ورکس میں کافی حد تک اوورلیپ ہے، لیکن ان کے ڈیزائن، صلاحیتوں، اور ہدف کے استعمال کے کیسز کے لحاظ سے کچھ اہم فرق ہیں:

- **AutoGen**: یہ ملٹی ایجنٹ سسٹمز پر جدید تحقیق کے لیے ایک تجرباتی فریم ورک ہے۔ یہ پیچیدہ ملٹی ایجنٹ سسٹمز کو پروٹوٹائپ کرنے اور تجربہ کرنے کے لیے بہترین جگہ ہے۔
- **Semantic Kernel**: یہ انٹرپرائز ایجنٹک ایپلیکیشنز بنانے کے لیے ایک پروڈکشن ریڈی ایجنٹ لائبریری ہے۔ یہ ایونٹ ڈرائیون، ڈسٹریبیوٹڈ ایجنٹک ایپلیکیشنز پر توجہ مرکوز کرتا ہے، جو متعدد LLMs اور SLMs، ٹولز، اور سنگل/ملٹی ایجنٹ ڈیزائن پیٹرنز کو فعال بناتا ہے۔
- **Azure AI Agent Service**: یہ Azure Foundry میں ایجنٹس کے لیے ایک پلیٹ فارم اور تعیناتی کی سروس ہے۔ یہ Azure Foundry کے ذریعے سپورٹ کیے جانے والے سروسز جیسے Azure OpenAI، Azure AI Search، Bing Search، اور کوڈ ایگزیکیوشن کے ساتھ کنیکٹیویٹی بنانے کی پیشکش کرتا ہے۔

اب بھی یقین نہیں کہ کون سا منتخب کریں؟

### استعمال کے کیسز

آئیے کچھ عام استعمال کے کیسز کے ذریعے آپ کی مدد کرنے کی کوشش کرتے ہیں:

> سوال: میں تجربہ کر رہا ہوں، سیکھ رہا ہوں اور پروف آف کانسیپٹ ایجنٹ ایپلیکیشنز بنا رہا ہوں، اور میں جلدی سے بنانا اور تجربہ کرنا چاہتا ہوں۔
>

> جواب: AutoGen اس منظرنامے کے لیے ایک اچھا انتخاب ہوگا، کیونکہ یہ ایونٹ ڈرائیون، ڈسٹریبیوٹڈ ایجنٹک ایپلیکیشنز پر توجہ مرکوز کرتا ہے اور جدید ملٹی ایجنٹ ڈیزائن پیٹرنز کو سپورٹ کرتا ہے۔

> سوال: اس استعمال کے کیس کے لیے AutoGen کو Semantic Kernel اور Azure AI Agent Service سے بہتر انتخاب کیا بناتا ہے؟
>
> جواب: AutoGen خاص طور پر ایونٹ ڈرائیون، ڈسٹریبیوٹڈ ایجنٹک ایپلیکیشنز کے لیے ڈیزائن کیا گیا ہے، جو اسے کوڈ جنریشن اور ڈیٹا اینالیسس کے کاموں کو خودکار بنانے کے لیے موزوں بناتا ہے۔ یہ پیچیدہ ملٹی ایجنٹ سسٹمز کو مؤثر طریقے سے بنانے کے لیے ضروری ٹولز اور صلاحیتیں فراہم کرتا ہے۔

> سوال: ایسا لگتا ہے کہ Azure AI Agent Service بھی یہاں کام کر سکتا ہے، اس میں کوڈ جنریشن اور مزید کے لیے ٹولز ہیں؟
>
> جواب: جی ہاں، Azure AI Agent Service ایجنٹس کے لیے ایک پلیٹ فارم سروس ہے اور متعدد ماڈلز، Azure AI Search، Bing Search، اور Azure Functions کے لیے بلٹ ان صلاحیتیں شامل کرتا ہے۔ یہ Foundry Portal میں آپ کے ایجنٹس کو بنانا اور انہیں اسکیل پر تعینات کرنا آسان بناتا ہے۔

> سوال: میں اب بھی الجھن میں ہوں، بس مجھے ایک آپشن دیں۔
>
> جواب: ایک بہترین انتخاب یہ ہے کہ آپ اپنی ایپلیکیشن Semantic Kernel میں بنائیں اور پھر Azure AI Agent Service کا استعمال کرتے ہوئے اپنے ایجنٹ کو تعینات کریں۔ یہ طریقہ آپ کو اپنے ایجنٹس کو آسانی سے برقرار رکھنے کی اجازت دیتا ہے جبکہ Semantic Kernel میں ملٹی ایجنٹ سسٹمز بنانے کی طاقت کا فائدہ اٹھاتا ہے۔ اس کے علاوہ، Semantic Kernel میں AutoGen کے لیے ایک کنیکٹر ہے، جو دونوں فریم ورکس کو ایک ساتھ استعمال کرنا آسان بناتا ہے۔

آئیے ایک ٹیبل میں کلیدی فرق کا خلاصہ کرتے ہیں:

| فریم ورک | توجہ | بنیادی تصورات | استعمال کے کیسز |
| --- | --- | --- | --- |
| AutoGen | ایونٹ ڈرائیون، ڈسٹریبیوٹڈ ایجنٹک ایپلیکیشنز | ایجنٹس، پرسونا، فنکشنز، ڈیٹا | کوڈ جنریشن، ڈیٹا اینالیسس کے کام |
| Semantic Kernel | انسانی جیسا ٹیکسٹ مواد سمجھنا اور بنانا | ایجنٹس، ماڈیولر کمپوننٹس، تعاون | نیچرل لینگویج انڈرسٹینڈنگ، مواد کی تخلیق |
| Azure AI Agent Service | لچکدار ماڈلز، انٹرپرائز سیکیورٹی، کوڈ جنریشن، ٹول کالنگ | ماڈیولریٹی، تعاون، پروسیس آرکیسٹریشن | محفوظ، اسکیل ایبل، اور لچکدار AI ایجنٹ کی تعیناتی |

ہر ایک فریم ورک کے لیے مثالی استعمال کا کیس کیا ہے؟

## کیا میں اپنے موجودہ Azure ایکوسسٹم ٹولز کو براہ راست انٹیگریٹ کر سکتا ہوں، یا مجھے اسٹینڈ الون سلوشنز کی ضرورت ہے؟

جواب ہاں میں ہے، آپ اپنے موجودہ Azure ایکوسسٹم ٹولز کو براہ راست Azure AI Agent Service کے ساتھ انٹیگریٹ کر سکتے ہیں، خاص طور پر اس لیے کہ یہ دیگر Azure سروسز کے ساتھ بغیر کسی رکاوٹ کے کام کرنے کے لیے بنایا گیا ہے۔ آپ مثال کے طور پر Bing، Azure AI Search، اور Azure Functions کو انٹیگریٹ کر سکتے ہیں۔ Azure AI Foundry کے ساتھ بھی گہری انٹیگریشن موجود ہے۔

AutoGen اور Semantic Kernel کے لیے، آپ Azure سروسز کے ساتھ انٹیگریٹ کر سکتے ہیں، لیکن اس کے لیے آپ کو اپنے کوڈ سے Azure سروسز کو کال کرنے کی ضرورت ہو سکتی ہے۔ انٹیگریٹ کرنے کا ایک اور طریقہ یہ ہے کہ Azure SDKs کا استعمال کرتے ہوئے اپنے ایجنٹس سے Azure سروسز کے ساتھ تعامل کریں۔ اس کے علاوہ، جیسا کہ ذکر کیا گیا، آپ Azure AI Agent Service کو AutoGen یا Semantic Kernel میں بنائے گئے ایجنٹس کے لیے آرکیسٹریٹر کے طور پر استعمال کر سکتے ہیں، جو Azure ایکوسسٹم تک آسان رسائی فراہم کرے گا۔

### AI Agent Frameworks کے بارے میں مزید سوالات ہیں؟

[Azure AI Foundry Discord](https://aka.ms/ai-agents/discord) میں شامل ہوں تاکہ دیگر سیکھنے والوں سے ملاقات کریں، آفس آورز میں شرکت کریں، اور اپنے AI ایجنٹس کے سوالات کے جوابات حاصل کریں۔

## حوالہ جات

- 

## پچھلا سبق

[AI ایجنٹس اور ان کے استعمال کے کیسز کا تعارف](../01-intro-to-ai-agents/README.md)

## اگلا سبق

[ایجنٹک ڈیزائن پیٹرنز کو سمجھنا](../03-agentic-design-patterns/README.md)

---

**ڈسکلیمر**:  
یہ دستاویز AI ترجمہ سروس [Co-op Translator](https://github.com/Azure/co-op-translator) کا استعمال کرتے ہوئے ترجمہ کی گئی ہے۔ ہم درستگی کے لیے پوری کوشش کرتے ہیں، لیکن براہ کرم آگاہ رہیں کہ خودکار ترجمے میں غلطیاں یا عدم درستگی ہو سکتی ہیں۔ اصل دستاویز کو اس کی اصل زبان میں مستند ذریعہ سمجھا جانا چاہیے۔ اہم معلومات کے لیے، پیشہ ور انسانی ترجمہ کی سفارش کی جاتی ہے۔ اس ترجمے کے استعمال سے پیدا ہونے والی کسی بھی غلط فہمی یا غلط تشریح کے لیے ہم ذمہ دار نہیں ہیں۔