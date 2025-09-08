<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-29T15:14:41+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "th"
}
-->
[![Exploring AI Agent Frameworks](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.th.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(คลิกที่ภาพด้านบนเพื่อดูวิดีโอของบทเรียนนี้)_

# สำรวจกรอบงาน AI Agent

กรอบงาน AI Agent คือแพลตฟอร์มซอฟต์แวร์ที่ออกแบบมาเพื่อช่วยให้การสร้าง การปรับใช้ และการจัดการ AI Agent เป็นเรื่องง่ายขึ้น กรอบงานเหล่านี้มอบส่วนประกอบที่สร้างไว้ล่วงหน้า เครื่องมือ และการจัดการที่ช่วยให้การพัฒนาระบบ AI ที่ซับซ้อนเป็นไปอย่างรวดเร็วและมีประสิทธิภาพ

กรอบงานเหล่านี้ช่วยให้นักพัฒนาสามารถมุ่งเน้นไปที่แง่มุมเฉพาะของแอปพลิเคชันของตน โดยใช้วิธีการมาตรฐานในการแก้ไขปัญหาทั่วไปในงานพัฒนา AI Agent ซึ่งช่วยเพิ่มความสามารถในการขยายตัว การเข้าถึง และประสิทธิภาพในการสร้างระบบ AI

## บทนำ

บทเรียนนี้จะครอบคลุม:

- กรอบงาน AI Agent คืออะไร และช่วยให้นักพัฒนาสามารถทำอะไรได้บ้าง?
- ทีมสามารถใช้กรอบงานเหล่านี้เพื่อสร้างต้นแบบอย่างรวดเร็ว ปรับปรุง และเพิ่มความสามารถของ Agent ได้อย่างไร?
- ความแตกต่างระหว่างกรอบงานและเครื่องมือที่ Microsoft สร้างขึ้นคืออะไร?
- ฉันสามารถผสานรวมเครื่องมือในระบบ Azure ที่มีอยู่ได้โดยตรง หรือจำเป็นต้องใช้โซลูชันแยกต่างหาก?
- บริการ Azure AI Agents คืออะไร และช่วยฉันได้อย่างไร?

## เป้าหมายการเรียนรู้

เป้าหมายของบทเรียนนี้คือช่วยให้คุณเข้าใจ:

- บทบาทของกรอบงาน AI Agent ในการพัฒนา AI
- วิธีใช้กรอบงาน AI Agent เพื่อสร้าง Agent ที่ชาญฉลาด
- ความสามารถสำคัญที่กรอบงาน AI Agent มอบให้
- ความแตกต่างระหว่าง AutoGen, Semantic Kernel และ Azure AI Agent Service

## กรอบงาน AI Agent คืออะไร และช่วยให้นักพัฒนาทำอะไรได้บ้าง?

กรอบงาน AI แบบดั้งเดิมสามารถช่วยให้คุณผสานรวม AI เข้ากับแอปของคุณและปรับปรุงแอปเหล่านี้ในลักษณะดังต่อไปนี้:

- **การปรับแต่งเฉพาะบุคคล**: AI สามารถวิเคราะห์พฤติกรรมและความชอบของผู้ใช้เพื่อมอบคำแนะนำ เนื้อหา และประสบการณ์ที่ปรับแต่งเฉพาะบุคคล
ตัวอย่าง: บริการสตรีมมิ่งอย่าง Netflix ใช้ AI เพื่อแนะนำภาพยนตร์และรายการทีวีตามประวัติการรับชม ซึ่งช่วยเพิ่มการมีส่วนร่วมและความพึงพอใจของผู้ใช้
- **การทำงานอัตโนมัติและประสิทธิภาพ**: AI สามารถทำงานซ้ำ ๆ โดยอัตโนมัติ ปรับปรุงกระบวนการทำงาน และเพิ่มประสิทธิภาพการดำเนินงาน
ตัวอย่าง: แอปบริการลูกค้าใช้แชทบอทที่ขับเคลื่อนด้วย AI เพื่อจัดการคำถามทั่วไป ลดเวลาตอบกลับ และช่วยให้เจ้าหน้าที่มนุษย์มีเวลาสำหรับปัญหาที่ซับซ้อนมากขึ้น
- **ประสบการณ์ผู้ใช้ที่ดีขึ้น**: AI สามารถปรับปรุงประสบการณ์ผู้ใช้โดยรวมด้วยการมอบฟีเจอร์อัจฉริยะ เช่น การจดจำเสียง การประมวลผลภาษาธรรมชาติ และข้อความคาดการณ์
ตัวอย่าง: ผู้ช่วยเสมือนอย่าง Siri และ Google Assistant ใช้ AI เพื่อเข้าใจและตอบสนองต่อคำสั่งเสียง ทำให้ผู้ใช้โต้ตอบกับอุปกรณ์ได้ง่ายขึ้น

### ฟังดูดีใช่ไหม แล้วทำไมเราถึงต้องการกรอบงาน AI Agent?

กรอบงาน AI Agent เป็นมากกว่ากรอบงาน AI ทั่วไป โดยออกแบบมาเพื่อสร้าง Agent ที่ชาญฉลาดซึ่งสามารถโต้ตอบกับผู้ใช้ Agent อื่น ๆ และสภาพแวดล้อมเพื่อบรรลุเป้าหมายเฉพาะ Agent เหล่านี้สามารถแสดงพฤติกรรมอัตโนมัติ ตัดสินใจ และปรับตัวให้เข้ากับสภาพแวดล้อมที่เปลี่ยนแปลงได้ ลองมาดูความสามารถสำคัญที่กรอบงาน AI Agent มอบให้:

- **การทำงานร่วมกันและการประสานงานของ Agent**: ช่วยสร้าง AI Agent หลายตัวที่สามารถทำงานร่วมกัน สื่อสาร และประสานงานเพื่อแก้ไขงานที่ซับซ้อน
- **การทำงานอัตโนมัติและการจัดการงาน**: มอบกลไกสำหรับการทำงานหลายขั้นตอนโดยอัตโนมัติ การมอบหมายงาน และการจัดการงานแบบไดนามิกระหว่าง Agent
- **ความเข้าใจและการปรับตัวตามบริบท**: มอบความสามารถให้ Agent เข้าใจบริบท ปรับตัวให้เข้ากับสภาพแวดล้อมที่เปลี่ยนแปลง และตัดสินใจตามข้อมูลแบบเรียลไทม์

สรุปคือ Agent ช่วยให้คุณทำสิ่งต่าง ๆ ได้มากขึ้น ยกระดับการทำงานอัตโนมัติไปอีกขั้น และสร้างระบบที่ชาญฉลาดขึ้นซึ่งสามารถปรับตัวและเรียนรู้จากสภาพแวดล้อม

## วิธีสร้างต้นแบบ ปรับปรุง และเพิ่มความสามารถของ Agent อย่างรวดเร็ว?

นี่เป็นพื้นที่ที่มีการเปลี่ยนแปลงอย่างรวดเร็ว แต่มีบางสิ่งที่เป็นเรื่องทั่วไปในกรอบงาน AI Agent ส่วนใหญ่ที่สามารถช่วยให้คุณสร้างต้นแบบและปรับปรุงได้อย่างรวดเร็ว ได้แก่ ส่วนประกอบแบบโมดูล เครื่องมือการทำงานร่วมกัน และการเรียนรู้แบบเรียลไทม์ ลองมาดูรายละเอียด:

- **ใช้ส่วนประกอบแบบโมดูล**: SDK AI มีส่วนประกอบที่สร้างไว้ล่วงหน้า เช่น ตัวเชื่อมต่อ AI และ Memory การเรียกฟังก์ชันโดยใช้ภาษาธรรมชาติหรือปลั๊กอินโค้ด เทมเพลตคำสั่ง และอื่น ๆ
- **ใช้เครื่องมือการทำงานร่วมกัน**: ออกแบบ Agent ที่มีบทบาทและงานเฉพาะ เพื่อทดสอบและปรับปรุงกระบวนการทำงานร่วมกัน
- **เรียนรู้แบบเรียลไทม์**: ใช้กลไกการตอบกลับที่ Agent เรียนรู้จากการโต้ตอบและปรับพฤติกรรมแบบไดนามิก

### ใช้ส่วนประกอบแบบโมดูล

SDK เช่น Microsoft Semantic Kernel และ LangChain มีส่วนประกอบที่สร้างไว้ล่วงหน้า เช่น ตัวเชื่อมต่อ AI เทมเพลตคำสั่ง และการจัดการหน่วยความจำ

**วิธีที่ทีมสามารถใช้สิ่งเหล่านี้**: ทีมสามารถประกอบส่วนประกอบเหล่านี้อย่างรวดเร็วเพื่อสร้างต้นแบบที่ใช้งานได้โดยไม่ต้องเริ่มต้นจากศูนย์ ซึ่งช่วยให้ทดลองและปรับปรุงได้อย่างรวดเร็ว

**วิธีการทำงานในทางปฏิบัติ**: คุณสามารถใช้ตัวแยกวิเคราะห์ที่สร้างไว้ล่วงหน้าเพื่อดึงข้อมูลจากการป้อนข้อมูลของผู้ใช้ โมดูลหน่วยความจำเพื่อจัดเก็บและดึงข้อมูล และตัวสร้างคำสั่งเพื่อโต้ตอบกับผู้ใช้ โดยไม่ต้องสร้างส่วนประกอบเหล่านี้ตั้งแต่ต้น

**ตัวอย่างโค้ด**. ลองดูตัวอย่างวิธีใช้ตัวเชื่อมต่อ AI ที่สร้างไว้ล่วงหน้ากับ Semantic Kernel Python และ .Net ที่ใช้การเรียกฟังก์ชันอัตโนมัติเพื่อให้โมเดลตอบสนองต่อการป้อนข้อมูลของผู้ใช้:

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

จากตัวอย่างนี้ คุณจะเห็นวิธีใช้ตัวแยกวิเคราะห์ที่สร้างไว้ล่วงหน้าเพื่อดึงข้อมูลสำคัญจากการป้อนข้อมูลของผู้ใช้ เช่น ต้นทาง ปลายทาง และวันที่ของคำขอจองเที่ยวบิน วิธีการแบบโมดูลนี้ช่วยให้คุณมุ่งเน้นไปที่ตรรกะระดับสูง

### ใช้เครื่องมือการทำงานร่วมกัน

กรอบงาน เช่น CrewAI, Microsoft AutoGen และ Semantic Kernel ช่วยให้สร้าง Agent หลายตัวที่สามารถทำงานร่วมกันได้

**วิธีที่ทีมสามารถใช้สิ่งเหล่านี้**: ทีมสามารถออกแบบ Agent ที่มีบทบาทและงานเฉพาะ เพื่อทดสอบและปรับปรุงกระบวนการทำงานร่วมกัน และเพิ่มประสิทธิภาพของระบบโดยรวม

**วิธีการทำงานในทางปฏิบัติ**: คุณสามารถสร้างทีม Agent ที่แต่ละตัวมีฟังก์ชันเฉพาะ เช่น การดึงข้อมูล การวิเคราะห์ หรือการตัดสินใจ Agent เหล่านี้สามารถสื่อสารและแบ่งปันข้อมูลเพื่อบรรลุเป้าหมายร่วมกัน เช่น การตอบคำถามของผู้ใช้หรือการทำงานให้เสร็จสมบูรณ์

**ตัวอย่างโค้ด (AutoGen)**:

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

ในโค้ดก่อนหน้านี้ คุณจะเห็นวิธีสร้างงานที่เกี่ยวข้องกับ Agent หลายตัวที่ทำงานร่วมกันเพื่อวิเคราะห์ข้อมูล แต่ละ Agent มีฟังก์ชันเฉพาะ และงานจะดำเนินการโดยการประสานงานระหว่าง Agent เพื่อให้ได้ผลลัพธ์ที่ต้องการ การสร้าง Agent เฉพาะที่มีบทบาทเฉพาะช่วยเพิ่มประสิทธิภาพและประสิทธิผลของงาน

### เรียนรู้แบบเรียลไทม์

กรอบงานขั้นสูงมอบความสามารถในการเข้าใจบริบทและปรับตัวแบบเรียลไทม์

**วิธีที่ทีมสามารถใช้สิ่งเหล่านี้**: ทีมสามารถใช้กลไกการตอบกลับที่ Agent เรียนรู้จากการโต้ตอบและปรับพฤติกรรมแบบไดนามิก ซึ่งนำไปสู่การปรับปรุงและการพัฒนาความสามารถอย่างต่อเนื่อง

**วิธีการทำงานในทางปฏิบัติ**: Agent สามารถวิเคราะห์ความคิดเห็นของผู้ใช้ ข้อมูลสิ่งแวดล้อม และผลลัพธ์ของงานเพื่ออัปเดตฐานความรู้ ปรับอัลกอริทึมการตัดสินใจ และปรับปรุงประสิทธิภาพเมื่อเวลาผ่านไป กระบวนการเรียนรู้แบบวนซ้ำนี้ช่วยให้ Agent ปรับตัวให้เข้ากับสภาพแวดล้อมที่เปลี่ยนแปลงและความชอบของผู้ใช้ ซึ่งช่วยเพิ่มประสิทธิภาพของระบบโดยรวม

## ความแตกต่างระหว่างกรอบงาน AutoGen, Semantic Kernel และ Azure AI Agent Service คืออะไร?

มีหลายวิธีในการเปรียบเทียบกรอบงานเหล่านี้ แต่ลองมาดูความแตกต่างสำคัญในแง่ของการออกแบบ ความสามารถ และกรณีการใช้งานเป้าหมาย:

## AutoGen

AutoGen เป็นกรอบงานโอเพ่นซอร์สที่พัฒนาโดย Microsoft Research's AI Frontiers Lab โดยมุ่งเน้นไปที่แอปพลิเคชันแบบกระจายที่ขับเคลื่อนด้วยเหตุการณ์ ซึ่งช่วยให้ LLM และ SLM หลายตัว เครื่องมือ และรูปแบบการออกแบบ Agent หลายตัวขั้นสูงทำงานร่วมกันได้

AutoGen สร้างขึ้นบนแนวคิดหลักของ Agent ซึ่งเป็นเอนทิตีอัตโนมัติที่สามารถรับรู้สภาพแวดล้อม ตัดสินใจ และดำเนินการเพื่อบรรลุเป้าหมายเฉพาะ Agent สื่อสารผ่านข้อความแบบอะซิงโครนัส ช่วยให้ทำงานได้อย่างอิสระและขนานกัน ซึ่งช่วยเพิ่มความสามารถในการขยายตัวและการตอบสนองของระบบ

. ตามที่ Wikipedia กล่าว Actor คือ _องค์ประกอบพื้นฐานของการคำนวณแบบขนาน ในการตอบสนองต่อข้อความที่ได้รับ Actor สามารถ: ตัดสินใจในพื้นที่ สร้าง Actor เพิ่มเติม ส่งข้อความเพิ่มเติม และกำหนดวิธีตอบสนองต่อข้อความถัดไปที่ได้รับ_

**กรณีการใช้งาน**: การสร้างโค้ดอัตโนมัติ งานวิเคราะห์ข้อมูล และการสร้าง Agent แบบกำหนดเองสำหรับฟังก์ชันการวางแผนและการวิจัย

นี่คือแนวคิดหลักที่สำคัญของ AutoGen:

- **Agent**. Agent คือเอนทิตีซอฟต์แวร์ที่:
  - **สื่อสารผ่านข้อความ** ซึ่งข้อความเหล่านี้สามารถเป็นแบบซิงโครนัสหรืออะซิงโครนัส
  - **รักษาสถานะของตัวเอง** ซึ่งสามารถเปลี่ยนแปลงได้โดยข้อความที่เข้ามา
  - **ดำเนินการ** เพื่อตอบสนองต่อข้อความที่ได้รับหรือการเปลี่ยนแปลงในสถานะของตัวเอง การดำเนินการเหล่านี้อาจเปลี่ยนแปลงสถานะของ Agent และสร้างผลกระทบภายนอก เช่น การอัปเดตบันทึกข้อความ การส่งข้อความใหม่ การดำเนินการโค้ด หรือการเรียก API

  นี่คือตัวอย่างโค้ดสั้น ๆ ที่คุณสร้าง Agent ของคุณเองที่มีความสามารถในการแชท:

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
    
    ในโค้ดก่อนหน้านี้ `MyAssistant` ถูกสร้างขึ้นและสืบทอดจาก `RoutedAgent` โดยมีตัวจัดการข้อความที่พิมพ์เนื้อหาของข้อความและส่งการตอบกลับโดยใช้ตัวแทน `AssistantAgent` โดยเฉพาะอย่างยิ่งสังเกตว่ามีการกำหนด `self._delegate` เป็นอินสแตนซ์ของ `AssistantAgent` ซึ่งเป็น Agent ที่สร้างไว้ล่วงหน้าที่สามารถจัดการการตอบกลับแชทได้

    มาทำให้ AutoGen รู้จักประเภท Agent นี้และเริ่มโปรแกรมกัน:

    ```python
    
    # main.py
    runtime = SingleThreadedAgentRuntime()
    await MyAgent.register(runtime, "my_agent", lambda: MyAgent())

    runtime.start()  # Start processing messages in the background.
    await runtime.send_message(MyMessageType("Hello, World!"), AgentId("my_agent", "default"))
    ```

    ในโค้ดก่อนหน้านี้ Agent ถูกลงทะเบียนกับ runtime และจากนั้นมีการส่งข้อความไปยัง Agent ซึ่งส่งผลให้ได้ผลลัพธ์ดังนี้:

    ```text
    # Output from the console:
    my_agent received message: Hello, World!
    my_assistant received message: Hello, World!
    my_assistant responded: Hello! How can I assist you today?
    ```

- **Agent หลายตัว**. AutoGen รองรับการสร้าง Agent หลายตัวที่สามารถทำงานร่วมกันเพื่อบรรลุงานที่ซับซ้อน Agent สามารถสื่อสาร แบ่งปันข้อมูล และประสานการกระทำของตนเพื่อแก้ปัญหาได้อย่างมีประสิทธิภาพมากขึ้น ในการสร้างระบบ Agent หลายตัว คุณสามารถกำหนดประเภท Agent ต่าง ๆ ที่มีฟังก์ชันและบทบาทเฉพาะ เช่น การดึงข้อมูล การวิเคราะห์ การตัดสินใจ และการโต้ตอบกับผู้ใช้ ลองดูตัวอย่างการสร้างดังกล่าวเพื่อให้เข้าใจ:

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

    ในโค้ดก่อนหน้านี้ เรามี `GroupChatManager` ที่ลงทะเบียนกับ runtime ผู้จัดการนี้รับผิดชอบในการประสานการโต้ตอบระหว่าง Agent ประเภทต่าง ๆ เช่น นักเขียน นักวาดภาพ บรรณาธิการ และผู้ใช้

- **Agent Runtime**. กรอบงานนี้มอบสภาพแวดล้อม runtime ที่ช่วยให้การสื่อสารระหว่าง Agent จัดการตัวตนและวงจรชีวิตของ Agent และบังคับใช้ขอบเขตความปลอดภัยและความเป็นส่วนตัว ซึ่งหมายความว่าคุณสามารถเรียกใช้ Agent ของคุณในสภาพแวดล้อมที่ปลอดภัยและควบคุมได้ เพื่อให้มั่นใจว่า Agent สามารถโต้ตอบได้อย่างปลอดภัยและมีประสิทธิภาพ มี runtime สองประเภทที่น่าสนใจ:
  - **Runtime แบบสแตนด์อโลน**. เป็นตัวเลือกที่ดีสำหรับแอปพลิเคชันที่ใช้กระบวนการเดียว ซึ่ง Agent ทั้งหมดถูกนำไปใช้ในภาษาโปรแกรมเดียวกันและทำงานในกระบวนการเดียวกัน นี่คือตัวอย่างการทำงาน:

    สแต็กแอปพลิเคชัน

    *Agent สื่อสารผ่านข้อความผ่าน runtime และ runtime จัดการวงจรชีวิตของ Agent*

  - **Runtime Agent แบบกระจาย**. เหมาะสำหรับแอปพลิเคชันที่ใช้หลายกระบวนการ ซึ่ง Agent อาจถูกนำไปใช้ในภาษาการเขียนโปรแกรมต่าง ๆ และทำงานบนเครื่องต่าง ๆ นี่คือตัวอย่างการทำงาน:

## Semantic Kernel + Agent Framework

Semantic Kernel เป็น SDK การจัดการ AI ที่พร้อมสำหรับองค์กร ประกอบด้วยตัวเชื่อมต่อ AI และ Memory พร้อมกับ Agent Framework

ลองมาดูส่วนประกอบหลัก:

- **ตัวเชื่อมต่อ AI**: เป็นอินเทอร์เฟซกับบริการ AI ภายนอกและแหล่งข้อมูลสำหรับใช้งานใน Python และ C#

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

    นี่คือตัวอย่างง่าย ๆ ของวิธีสร้าง Kernel และเพิ่มบริการแชทคอมพลีชั่น Semantic Kernel สร้างการเชื่อมต่อกับบริการ AI ภายนอก ในกรณีนี้คือ Azure OpenAI Chat Completion

- **ปลั๊กอิน**: ปลั๊กอินเหล่านี้ครอบคลุมฟังก์ชันที่แอปพลิเคชันสามารถใช้ได้ มีทั้งปลั๊กอินที่สร้างไว้ล่วงหน้าและปลั๊กอินที่คุณสามารถสร้างเองได้ แนวคิดที่เกี่ยวข้องคือ "ฟังก์ชันคำสั่ง" แทนที่จะให้คำแนะนำภาษาธรรมชาติสำหรับการเรียกฟังก์ชัน คุณสามารถเผยแพร่ฟังก์ชันบางอย่างไปยังโมเดลได้ โดยขึ้นอยู่กับบริบทการแชทปัจจุบัน โมเดลอาจเลือกเรียกหนึ่งในฟังก์ชันเหล่านี้เพื่อทำคำขอหรือคำถามให้เสร็จสมบูรณ์ นี่คือตัวอย่าง:

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

    ในที่นี้ คุณมีเทมเพลตคำสั่ง `skPrompt` ที่เว้นที่ว่างให้ผู้ใช้ป้อนข้อความ `$userInput` จากนั้นคุณสร้างฟังก์
## บริการ Azure AI Agent

Azure AI Agent Service เป็นฟีเจอร์ใหม่ที่เปิดตัวในงาน Microsoft Ignite 2024 ช่วยให้สามารถพัฒนาและปรับใช้ AI agents ด้วยโมเดลที่ยืดหยุ่นมากขึ้น เช่น การเรียกใช้งาน LLMs แบบโอเพ่นซอร์สโดยตรง เช่น Llama 3, Mistral และ Cohere

Azure AI Agent Service มาพร้อมกับกลไกความปลอดภัยระดับองค์กรและวิธีการจัดเก็บข้อมูลที่แข็งแกร่ง ทำให้เหมาะสำหรับการใช้งานในองค์กร

บริการนี้สามารถใช้งานร่วมกับเฟรมเวิร์กการจัดการหลายเอเจนต์ เช่น AutoGen และ Semantic Kernel ได้ทันที

ปัจจุบันบริการนี้อยู่ในช่วง Public Preview และรองรับการพัฒนาเอเจนต์ด้วย Python และ C#

โดยใช้ Semantic Kernel Python เราสามารถสร้าง Azure AI Agent พร้อมปลั๊กอินที่กำหนดเองได้ดังนี้:

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

### แนวคิดหลัก

Azure AI Agent Service มีแนวคิดหลักดังนี้:

- **Agent**. Azure AI Agent Service ผสานรวมกับ Azure AI Foundry ภายใน AI Foundry, AI Agent ทำหน้าที่เป็น "ไมโครเซอร์วิสอัจฉริยะ" ที่สามารถใช้ตอบคำถาม (RAG) ดำเนินการ หรือทำงานอัตโนมัติได้อย่างสมบูรณ์ โดยใช้พลังของโมเดล AI เชิงสร้างสรรค์ร่วมกับเครื่องมือที่ช่วยให้เข้าถึงและโต้ตอบกับแหล่งข้อมูลในโลกจริงได้ ตัวอย่างของเอเจนต์มีดังนี้:

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    ในตัวอย่างนี้ เอเจนต์ถูกสร้างขึ้นด้วยโมเดล `gpt-4o-mini` ชื่อ `my-agent` และคำแนะนำ `You are helpful agent` เอเจนต์นี้มีเครื่องมือและทรัพยากรที่พร้อมสำหรับการทำงานด้านการตีความโค้ด

- **Thread และข้อความ**. Thread เป็นอีกหนึ่งแนวคิดสำคัญ มันแสดงถึงการสนทนาหรือการโต้ตอบระหว่างเอเจนต์และผู้ใช้ Threads สามารถใช้เพื่อติดตามความคืบหน้าของการสนทนา เก็บข้อมูลบริบท และจัดการสถานะของการโต้ตอบ ตัวอย่างของ Thread มีดังนี้:

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

    ในโค้ดข้างต้น Thread ถูกสร้างขึ้น จากนั้นมีการส่งข้อความไปยัง Thread โดยการเรียก `create_and_process_run` เอเจนต์จะถูกขอให้ทำงานใน Thread สุดท้าย ข้อความจะถูกดึงและบันทึกเพื่อตรวจสอบการตอบสนองของเอเจนต์ ข้อความเหล่านี้แสดงถึงความคืบหน้าของการสนทนาระหว่างผู้ใช้และเอเจนต์ นอกจากนี้ยังสำคัญที่ต้องเข้าใจว่าข้อความสามารถมีหลายประเภท เช่น ข้อความตัวอักษร รูปภาพ หรือไฟล์ ซึ่งเป็นผลลัพธ์จากการทำงานของเอเจนต์ เช่น การตอบกลับเป็นข้อความหรือรูปภาพ นักพัฒนาสามารถใช้ข้อมูลนี้เพื่อประมวลผลเพิ่มเติมหรือแสดงผลให้ผู้ใช้

- **การผสานรวมกับเฟรมเวิร์ก AI อื่นๆ**. Azure AI Agent Service สามารถโต้ตอบกับเฟรมเวิร์กอื่นๆ เช่น AutoGen และ Semantic Kernel ซึ่งหมายความว่าคุณสามารถสร้างส่วนหนึ่งของแอปในเฟรมเวิร์กเหล่านี้ และใช้ Agent Service เป็นตัวจัดการ หรือสร้างทุกอย่างใน Agent Service ได้

**กรณีการใช้งาน**: Azure AI Agent Service ถูกออกแบบมาสำหรับแอปพลิเคชันในองค์กรที่ต้องการการปรับใช้ AI agent ที่ปลอดภัย ขยายขนาดได้ และยืดหยุ่น

## ความแตกต่างระหว่างเฟรมเวิร์กเหล่านี้คืออะไร?

ดูเหมือนว่าเฟรมเวิร์กเหล่านี้จะมีความซ้อนทับกันอยู่บ้าง แต่ก็มีความแตกต่างสำคัญในแง่ของการออกแบบ ความสามารถ และกรณีการใช้งานเป้าหมาย:

- **AutoGen**: เป็นเฟรมเวิร์กสำหรับการทดลองที่เน้นการวิจัยล้ำสมัยเกี่ยวกับระบบหลายเอเจนต์ เหมาะสำหรับการทดลองและสร้างต้นแบบระบบหลายเอเจนต์ที่ซับซ้อน
- **Semantic Kernel**: เป็นไลบรารีเอเจนต์ที่พร้อมใช้งานในระดับการผลิตสำหรับการสร้างแอปพลิเคชันเอเจนต์ในองค์กร เน้นแอปพลิเคชันที่ขับเคลื่อนด้วยเหตุการณ์และกระจายตัว รองรับ LLMs และ SLMs หลายตัว เครื่องมือ และรูปแบบการออกแบบเอเจนต์เดี่ยว/หลายตัว
- **Azure AI Agent Service**: เป็นแพลตฟอร์มและบริการปรับใช้ใน Azure Foundry สำหรับเอเจนต์ มีการเชื่อมต่อกับบริการต่างๆ ที่ Azure รองรับ เช่น Azure OpenAI, Azure AI Search, Bing Search และการรันโค้ด

ยังไม่แน่ใจว่าจะเลือกอะไรดี?

### กรณีการใช้งาน

ลองดูกรณีการใช้งานทั่วไปเพื่อช่วยคุณตัดสินใจ:

> Q: ฉันกำลังทดลอง เรียนรู้ และสร้างแอปพลิเคชันเอเจนต์ต้นแบบ และต้องการสร้างและทดลองได้อย่างรวดเร็ว
>

>A: AutoGen จะเป็นตัวเลือกที่ดีสำหรับสถานการณ์นี้ เนื่องจากเน้นแอปพลิเคชันเอเจนต์ที่ขับเคลื่อนด้วยเหตุการณ์และกระจายตัว และรองรับรูปแบบการออกแบบหลายเอเจนต์ขั้นสูง

> Q: อะไรทำให้ AutoGen เป็นตัวเลือกที่ดีกว่า Semantic Kernel และ Azure AI Agent Service สำหรับกรณีนี้?
>
> A: AutoGen ถูกออกแบบมาโดยเฉพาะสำหรับแอปพลิเคชันเอเจนต์ที่ขับเคลื่อนด้วยเหตุการณ์และกระจายตัว ทำให้เหมาะสำหรับการทำงานอัตโนมัติในงานสร้างโค้ดและวิเคราะห์ข้อมูล มันมีเครื่องมือและความสามารถที่จำเป็นสำหรับการสร้างระบบหลายเอเจนต์ที่ซับซ้อนอย่างมีประสิทธิภาพ

>Q: ฟังดูเหมือน Azure AI Agent Service ก็สามารถใช้งานได้ในกรณีนี้เช่นกัน เพราะมีเครื่องมือสำหรับการสร้างโค้ดและอื่นๆ ใช่ไหม?

>
> A: ใช่ Azure AI Agent Service เป็นแพลตฟอร์มบริการสำหรับเอเจนต์ และมีความสามารถในตัวสำหรับโมเดลหลายตัว, Azure AI Search, Bing Search และ Azure Functions ทำให้ง่ายต่อการสร้างเอเจนต์ใน Foundry Portal และปรับใช้ในขนาดใหญ่

> Q: ฉันยังสับสนอยู่ แค่บอกตัวเลือกเดียวให้ฉัน
>
> A: ตัวเลือกที่ดีคือการสร้างแอปพลิเคชันของคุณใน Semantic Kernel ก่อน แล้วจึงใช้ Azure AI Agent Service เพื่อปรับใช้เอเจนต์ของคุณ วิธีนี้ช่วยให้คุณสามารถเก็บเอเจนต์ของคุณได้ง่าย ในขณะที่ใช้พลังของการสร้างระบบหลายเอเจนต์ใน Semantic Kernel นอกจากนี้ Semantic Kernel ยังมีตัวเชื่อมต่อใน AutoGen ทำให้ง่ายต่อการใช้เฟรมเวิร์กทั้งสองร่วมกัน

ลองสรุปความแตกต่างสำคัญในตาราง:

| เฟรมเวิร์ก | จุดเน้น | แนวคิดหลัก | กรณีการใช้งาน |
| --- | --- | --- | --- |
| AutoGen | แอปพลิเคชันเอเจนต์ที่ขับเคลื่อนด้วยเหตุการณ์และกระจายตัว | Agents, Personas, Functions, Data | การสร้างโค้ด, งานวิเคราะห์ข้อมูล |
| Semantic Kernel | การทำความเข้าใจและสร้างเนื้อหาที่เหมือนมนุษย์ | Agents, Modular Components, Collaboration | การทำความเข้าใจภาษาธรรมชาติ, การสร้างเนื้อหา |
| Azure AI Agent Service | โมเดลที่ยืดหยุ่น, ความปลอดภัยระดับองค์กร, การสร้างโค้ด, การเรียกใช้เครื่องมือ | Modularity, Collaboration, Process Orchestration | การปรับใช้ AI agent ที่ปลอดภัย ขยายขนาดได้ และยืดหยุ่น |

กรณีการใช้งานที่เหมาะสมที่สุดสำหรับแต่ละเฟรมเวิร์กคืออะไร?

## ฉันสามารถผสานรวมเครื่องมือในระบบ Azure ที่มีอยู่ได้โดยตรง หรือจำเป็นต้องใช้โซลูชันแยกต่างหาก?

คำตอบคือได้ คุณสามารถผสานรวมเครื่องมือในระบบ Azure ที่มีอยู่ได้โดยตรงกับ Azure AI Agent Service โดยเฉพาะ เนื่องจากมันถูกสร้างมาให้ทำงานร่วมกับบริการ Azure อื่นๆ ได้อย่างราบรื่น ตัวอย่างเช่น คุณสามารถผสานรวม Bing, Azure AI Search และ Azure Functions นอกจากนี้ยังมีการผสานรวมลึกซึ้งกับ Azure AI Foundry

สำหรับ AutoGen และ Semantic Kernel คุณก็สามารถผสานรวมกับบริการ Azure ได้เช่นกัน แต่คุณอาจต้องเรียกใช้บริการ Azure จากโค้ดของคุณ อีกวิธีหนึ่งคือการใช้ Azure SDKs เพื่อโต้ตอบกับบริการ Azure จากเอเจนต์ของคุณ นอกจากนี้ อย่างที่กล่าวไป คุณสามารถใช้ Azure AI Agent Service เป็นตัวจัดการสำหรับเอเจนต์ที่สร้างใน AutoGen หรือ Semantic Kernel ซึ่งจะช่วยให้เข้าถึงระบบ Azure ได้ง่าย

### มีคำถามเพิ่มเติมเกี่ยวกับ AI Agent Frameworks ไหม?

เข้าร่วม [Azure AI Foundry Discord](https://aka.ms/ai-agents/discord) เพื่อพบปะกับผู้เรียนคนอื่นๆ เข้าร่วมชั่วโมงให้คำปรึกษา และรับคำตอบสำหรับคำถามเกี่ยวกับ AI Agents ของคุณ

## อ้างอิง

- 

## บทเรียนก่อนหน้า

[Introduction to AI Agents and Agent Use Cases](../01-intro-to-ai-agents/README.md)

## บทเรียนถัดไป

[Understanding Agentic Design Patterns](../03-agentic-design-patterns/README.md)

---

**ข้อจำกัดความรับผิดชอบ**:  
เอกสารนี้ได้รับการแปลโดยใช้บริการแปลภาษา AI [Co-op Translator](https://github.com/Azure/co-op-translator) แม้ว่าเราจะพยายามให้การแปลมีความถูกต้อง แต่โปรดทราบว่าการแปลอัตโนมัติอาจมีข้อผิดพลาดหรือความไม่แม่นยำ เอกสารต้นฉบับในภาษาต้นทางควรถือเป็นแหล่งข้อมูลที่เชื่อถือได้ สำหรับข้อมูลที่สำคัญ ขอแนะนำให้ใช้บริการแปลภาษามนุษย์มืออาชีพ เราจะไม่รับผิดชอบต่อความเข้าใจผิดหรือการตีความที่ผิดพลาดซึ่งเกิดจากการใช้การแปลนี้