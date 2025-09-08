<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "a9631d0898fc3c6ecbb3a8a0da7aaba3",
  "translation_date": "2025-08-28T09:22:11+00:00",
  "source_file": "02-explore-agentic-frameworks/README.md",
  "language_code": "tw"
}
-->
[![探索 AI Agent 框架](../../../translated_images/lesson-2-thumbnail.c65f44c93b8558df4d5d407e29970e654629e614f357444a9c27c80feb54c79d.tw.png)](https://youtu.be/ODwF-EZo_O8?si=1xoy_B9RNQfrYdF7)

> _(點擊上方圖片觀看本課程的影片)_

# 探索 AI Agent 框架

AI Agent 框架是專為簡化 AI Agent 的創建、部署和管理而設計的軟體平台。這些框架為開發者提供了預建的元件、抽象層和工具，從而加速複雜 AI 系統的開發。

這些框架通過提供標準化的方法來解決 AI Agent 開發中的常見挑戰，幫助開發者專注於應用程式的獨特部分。它們提升了 AI 系統的可擴展性、可訪問性和效率。

## 簡介

本課程將涵蓋：

- 什麼是 AI Agent 框架？它們能幫助開發者實現什麼？
- 團隊如何利用這些框架快速原型設計、迭代並提升 Agent 的能力？
- 微軟開發的框架和工具之間有什麼不同？
- 我是否可以直接整合現有的 Azure 生態系統工具，還是需要獨立的解決方案？
- 什麼是 Azure AI Agents 服務？它如何幫助我？

## 學習目標

本課程的目標是幫助你理解：

- AI Agent 框架在 AI 開發中的角色。
- 如何利用 AI Agent 框架構建智能 Agent。
- AI Agent 框架所啟用的關鍵功能。
- AutoGen、Semantic Kernel 和 Azure AI Agent Service 之間的差異。

## 什麼是 AI Agent 框架？它們能幫助開發者做什麼？

傳統的 AI 框架可以幫助你將 AI 整合到應用程式中，並通過以下方式改進這些應用程式：

- **個性化**：AI 可以分析用戶行為和偏好，提供個性化的推薦、內容和體驗。
  範例：像 Netflix 這樣的串流服務利用 AI 根據觀看歷史推薦電影和節目，提升用戶參與度和滿意度。
- **自動化與效率**：AI 可以自動化重複性任務、簡化工作流程並提高運營效率。
  範例：客戶服務應用程式使用 AI 驅動的聊天機器人處理常見查詢，縮短響應時間，並讓人類客服專注於更複雜的問題。
- **提升用戶體驗**：AI 可以通過提供智能功能（如語音識別、自然語言處理和預測文本）來改善整體用戶體驗。
  範例：像 Siri 和 Google Assistant 這樣的虛擬助手利用 AI 理解並響應語音指令，使用戶更輕鬆地與設備互動。

### 聽起來很棒，為什麼還需要 AI Agent 框架？

AI Agent 框架不僅僅是 AI 框架，它們旨在創建能與用戶、其他 Agent 和環境互動以實現特定目標的智能 Agent。這些 Agent 可以表現出自主行為、做出決策並適應變化的條件。以下是 AI Agent 框架啟用的一些關鍵功能：

- **Agent 協作與協調**：支持創建多個 AI Agent，它們可以協作、溝通並協調以解決複雜任務。
- **任務自動化與管理**：提供自動化多步工作流程、任務分配和 Agent 間動態任務管理的機制。
- **情境理解與適應**：使 Agent 能夠理解情境、適應變化的環境，並根據實時資訊做出決策。

總而言之，Agent 讓你能做得更多，將自動化提升到新的層次，創建能從環境中學習並適應的更智能系統。

## 如何快速原型設計、迭代並提升 Agent 的能力？

這是一個快速變化的領域，但大多數 AI Agent 框架都有一些共同點，可以幫助你快速原型設計和迭代，主要包括模組化元件、協作工具和實時學習。讓我們深入了解這些：

- **使用模組化元件**：AI SDK 提供預建的元件，例如 AI 和記憶體連接器、使用自然語言或程式碼插件進行函數調用、提示模板等。
- **利用協作工具**：設計具有特定角色和任務的 Agent，從而測試和完善協作工作流程。
- **實時學習**：實施反饋迴路，讓 Agent 從互動中學習並動態調整其行為。

### 使用模組化元件

像 Microsoft Semantic Kernel 和 LangChain 這樣的 SDK 提供了預建的元件，例如 AI 連接器、提示模板和記憶體管理。

**團隊如何使用這些元件**：團隊可以快速組裝這些元件來創建功能性原型，而無需從頭開始，從而實現快速實驗和迭代。

**實際運作方式**：你可以使用預建的解析器從用戶輸入中提取資訊，使用記憶體模組存儲和檢索數據，並使用提示生成器與用戶互動，而無需從頭構建這些元件。

**範例程式碼**。以下是如何使用 Semantic Kernel Python 和 .Net 的預建 AI 連接器的範例，該連接器使用自動函數調用來讓模型響應用戶輸入：

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

從這個範例中可以看到，你如何利用預建的解析器從用戶輸入中提取關鍵資訊，例如航班預訂請求的出發地、目的地和日期。這種模組化方法讓你能專注於高層邏輯。

### 利用協作工具

像 CrewAI、Microsoft AutoGen 和 Semantic Kernel 這樣的框架促進了多個 Agent 的創建，這些 Agent 可以協作完成任務。

**團隊如何使用這些工具**：團隊可以設計具有特定角色和任務的 Agent，從而測試和完善協作工作流程，並提高整體系統效率。

**實際運作方式**：你可以創建一組 Agent，每個 Agent 都有專門的功能，例如數據檢索、分析或決策。這些 Agent 可以溝通並共享資訊，以實現共同目標，例如回答用戶查詢或完成任務。

**範例程式碼 (AutoGen)**：

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

在上述程式碼中，你可以看到如何創建一個涉及多個 Agent 協作分析數據的任務。每個 Agent 執行特定功能，並通過協調這些 Agent 來完成所需的結果。通過創建具有專門角色的專用 Agent，你可以提高任務效率和性能。

### 實時學習

高級框架提供了實時情境理解和適應的功能。

**團隊如何使用這些功能**：團隊可以實施反饋迴路，讓 Agent 從互動中學習並動態調整其行為，從而實現能力的持續改進和完善。

**實際運作方式**：Agent 可以分析用戶反饋、環境數據和任務結果，更新其知識庫、調整決策演算法並隨時間改進性能。這種迭代學習過程使 Agent 能夠適應變化的條件和用戶偏好，提升整體系統的有效性。

## AutoGen、Semantic Kernel 和 Azure AI Agent Service 框架之間有什麼不同？

比較這些框架的方法有很多，但我們來看看它們在設計、功能和目標使用案例方面的一些關鍵差異：

## AutoGen

AutoGen 是由微軟研究院的 AI Frontiers Lab 開發的開源框架。它專注於事件驅動的分散式 *agentic* 應用程式，支持多個 LLM 和 SLM、工具以及高級多 Agent 設計模式。

AutoGen 的核心概念是 Agent，它是能夠感知環境、做出決策並採取行動以實現特定目標的自主實體。Agent 通過非同步消息進行通信，使它們能夠獨立並行工作，從而提高系統的可擴展性和響應性。

根據維基百科的定義，Actor 是 _並行計算的基本構建塊。收到消息後，Actor 可以：做出本地決策、創建更多 Actor、發送更多消息，並決定如何響應下一條收到的消息_。

**使用案例**：自動化程式碼生成、數據分析任務，以及為規劃和研究功能構建自定義 Agent。

以下是 AutoGen 的一些重要核心概念：

- **Agent**。Agent 是一種軟體實體，具有以下特性：
  - **通過消息進行通信**，這些消息可以是同步或非同步的。
  - **維護自己的狀態**，該狀態可以通過接收到的消息進行修改。
  - **執行動作**，以響應接收到的消息或其狀態的變化。這些動作可能會修改 Agent 的狀態並產生外部效果，例如更新消息日誌、發送新消息、執行程式碼或進行 API 調用。

  以下是一段簡短的程式碼範例，展示如何創建具有聊天功能的 Agent：

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

    在上述程式碼中，`MyAssistant` 被創建並繼承自 `RoutedAgent`。它有一個消息處理器，該處理器會打印消息內容，然後使用 `AssistantAgent` 委派發送回應。特別需要注意的是，我們將 `self._delegate` 指定為 `AssistantAgent` 的實例，這是一個預建的 Agent，能處理聊天完成。

    接下來，讓 AutoGen 知道這種類型的 Agent 並啟動程式：

    ```python
    
    # main.py
    runtime = SingleThreadedAgentRuntime()
    await MyAgent.register(runtime, "my_agent", lambda: MyAgent())

    runtime.start()  # Start processing messages in the background.
    await runtime.send_message(MyMessageType("Hello, World!"), AgentId("my_agent", "default"))
    ```

    在上述程式碼中，Agent 被註冊到運行時，然後向 Agent 發送一條消息，結果輸出如下：

    ```text
    # Output from the console:
    my_agent received message: Hello, World!
    my_assistant received message: Hello, World!
    my_assistant responded: Hello! How can I assist you today?
    ```

- **多 Agent**。AutoGen 支持創建多個 Agent，它們可以協作完成複雜任務。Agent 可以通信、共享資訊並協調行動，以更高效地解決問題。要創建多 Agent 系統，你可以定義具有專門功能和角色的不同類型的 Agent，例如數據檢索、分析、決策和用戶互動。以下是這樣的創建範例：

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

    在上述程式碼中，我們有一個 `GroupChatManager`，它被註冊到運行時。該管理器負責協調不同類型 Agent（如作家、插畫家、編輯和用戶）之間的互動。

- **Agent 運行時**。該框架提供了一個運行時環境，支持 Agent 之間的通信，管理它們的身份和生命週期，並強制執行安全和隱私邊界。這意味著你可以在安全受控的環境中運行 Agent，確保它們能夠安全高效地互動。這裡有兩種運行時值得關注：
  - **獨立運行時**。適用於所有 Agent 都用相同程式語言實現並運行在同一進程中的單進程應用程式。其運作方式如下：

    應用程式堆疊

    *Agent 通過運行時進行消息通信，運行時管理 Agent 的生命週期*

  - **分散式 Agent 運行時**。適用於多進程應用程式，其中 Agent 可以用不同的程式語言實現並運行在不同的機器上。其運作方式如下：

## Semantic Kernel + Agent Framework

Semantic Kernel 是一個企業級的 AI 編排 SDK。它由 AI 和記憶體連接器以及一個 Agent 框架組成。

首先讓我們了解一些核心元件：

- **AI 連接器**：這是一個用於與外部 AI 服務和數據源進行介面的工具，支持 Python 和 C#。

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

    這裡是一個簡單的範例，展示如何創建一個 Kernel 並添加聊天完成服務。Semantic Kernel 創建了一個與外部 AI 服務（此處為 Azure OpenAI Chat Completion）的連接。

- **插件**：這些封裝了應用程式可以使用的功能。既有現成的插件，也可以創建自定義插件。一個相關的概念是「提示函數」。與提供自然語言提示來調用函數不同，你可以向模型廣播某些函數。根據當前聊天上下文，模型可能會選擇調用這些函數之一來完成請求或查詢。以下是一個範例：

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

    在這裡，你首先有一個模板提示 `skPrompt`，它為用戶輸入文本 `$userInput` 留出了空間。然後你創建了 Kernel 函數 `SummarizeText`，並將其作為插件名稱 `SemanticFunctions` 導入到 Kernel 中。函數的名稱幫助 Semantic Kernel 理解該函數的作用以及何時應該調用它。

- **原生函數**：框架還可以直接調用原生函數來執行任務。以下是一個範例，展示如何從文件中檢索內容：

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

- **記憶體**：抽象並簡化了 AI 應用程式的上下文管理。記憶體的概念是 LLM 應該知道的內容。你可以將這些資訊存儲在向量存儲中，這最終是一個內存數據庫或向量數據庫或類似的東西。以下是一個非常簡化的場景範例，展示如何將 *事實* 添加到記憶體中：

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

    這些事實然後被存儲在記憶體集合 `SummarizedAzureDocs` 中。這是一個非常簡化的範例，但你可以看到如何將資訊存儲在記憶體中供 LLM 使用。
## Azure AI Agent Service

Azure AI Agent Service 是一個較新的功能，於 2024 年 Microsoft Ignite 大會上推出。它允許開發和部署具有更靈活模型的 AI Agent，例如直接調用開源的 LLM（如 Llama 3、Mistral 和 Cohere）。

Azure AI Agent Service 提供更強大的企業安全機制和數據存儲方法，非常適合企業應用。

它可以與多代理協作框架（如 AutoGen 和 Semantic Kernel）即時搭配使用。

該服務目前處於公開預覽階段，支持使用 Python 和 C# 來構建代理。

使用 Semantic Kernel 的 Python，我們可以通過用戶定義的插件創建一個 Azure AI Agent：

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

### 核心概念

Azure AI Agent Service 包含以下核心概念：

- **Agent（代理）**。Azure AI Agent Service 與 Azure AI Foundry 集成。在 AI Foundry 中，AI Agent 作為一個「智能」微服務，可以用來回答問題（RAG）、執行操作或完全自動化工作流程。它通過結合生成式 AI 模型的能力與能夠訪問和交互真實數據源的工具來實現這些功能。以下是一個代理的示例：

    ```python
    agent = project_client.agents.create_agent(
        model="gpt-4o-mini",
        name="my-agent",
        instructions="You are helpful agent",
        tools=code_interpreter.definitions,
        tool_resources=code_interpreter.resources,
    )
    ```

    在這個示例中，創建了一個代理，使用模型 `gpt-4o-mini`，名稱為 `my-agent`，指令為 `You are helpful agent`。該代理配備了執行代碼解釋任務的工具和資源。

- **Thread（線程）和 Messages（消息）**。線程是另一個重要的概念。它表示代理與用戶之間的對話或交互。線程可用於跟蹤對話進度、存儲上下文信息以及管理交互的狀態。以下是一個線程的示例：

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

    在上述代碼中，創建了一個線程。隨後，一條消息被發送到該線程。通過調用 `create_and_process_run`，代理被要求在該線程上執行工作。最後，消息被提取並記錄下來以查看代理的回應。這些消息表明了用戶與代理之間對話的進展。需要注意的是，消息可以是不同類型的，例如文本、圖片或文件，這些是代理工作的結果，例如生成了一張圖片或一段文本回應。作為開發者，你可以使用這些信息進一步處理回應或將其展示給用戶。

- **與其他 AI 框架集成**。Azure AI Agent Service 可以與其他框架（如 AutoGen 和 Semantic Kernel）交互，這意味著你可以在這些框架之一中構建部分應用，並使用 Agent Service 作為協調器，或者完全在 Agent Service 中構建應用。

**使用場景**：Azure AI Agent Service 專為需要安全、可擴展和靈活的 AI Agent 部署的企業應用而設計。

## 這些框架之間有什麼區別？

看起來這些框架之間有很多重疊，但它們在設計、功能和目標使用場景方面有一些關鍵區別：

- **AutoGen**：是一個專注於多代理系統前沿研究的實驗框架。它是實驗和原型設計複雜多代理系統的最佳選擇。
- **Semantic Kernel**：是一個面向生產的代理庫，用於構建企業級代理應用。專注於事件驅動的分佈式代理應用，支持多個 LLM 和 SLM、工具以及單/多代理設計模式。
- **Azure AI Agent Service**：是一個 Azure Foundry 中的代理平台和部署服務。它提供與 Azure Foundry 支持的服務（如 Azure OpenAI、Azure AI Search、Bing Search 和代碼執行）的連接能力。

還是不確定該選哪一個？

### 使用場景

讓我們通過一些常見的使用場景來幫助你做出選擇：

> 問：我正在進行實驗、學習並構建概念驗證的代理應用，我希望能快速構建和實驗。
>

> 答：AutoGen 是這種情況下的好選擇，因為它專注於事件驅動的分佈式代理應用，並支持高級多代理設計模式。

> 問：為什麼在這種使用場景下，AutoGen 比 Semantic Kernel 和 Azure AI Agent Service 更好？
>
> 答：AutoGen 專為事件驅動的分佈式代理應用設計，非常適合自動化代碼生成和數據分析任務。它提供了構建複雜多代理系統所需的工具和功能。

> 問：聽起來 Azure AI Agent Service 也可以用於這種情況，它有代碼生成等工具？
>
> 答：是的，Azure AI Agent Service 是一個代理平台服務，內置支持多個模型、Azure AI Search、Bing Search 和 Azure Functions。它使你能夠輕鬆在 Foundry Portal 中構建代理並進行大規模部署。

> 問：我還是有點困惑，能不能給我一個簡單的選擇？
>
> 答：一個不錯的選擇是先在 Semantic Kernel 中構建你的應用，然後使用 Azure AI Agent Service 部署你的代理。這種方法使你能夠輕鬆持久化你的代理，同時利用 Semantic Kernel 構建多代理系統的能力。此外，Semantic Kernel 在 AutoGen 中有一個連接器，使得同時使用這兩個框架變得簡單。

讓我們用一個表格來總結這些框架的主要區別：

| 框架 | 重點 | 核心概念 | 使用場景 |
| --- | --- | --- | --- |
| AutoGen | 事件驅動的分佈式代理應用 | Agents, Personas, Functions, Data | 代碼生成、數據分析任務 |
| Semantic Kernel | 理解和生成類人文本內容 | Agents, Modular Components, Collaboration | 自然語言理解、內容生成 |
| Azure AI Agent Service | 靈活模型、企業安全、代碼生成、工具調用 | Modularity, Collaboration, Process Orchestration | 安全、可擴展且靈活的 AI Agent 部署 |

每個框架的理想使用場景是什麼？

## 我可以直接集成現有的 Azure 生態系統工具，還是需要獨立解決方案？

答案是肯定的，你可以直接將現有的 Azure 生態系統工具與 Azure AI Agent Service 集成，因為它被設計為能與其他 Azure 服務無縫協作。例如，你可以集成 Bing、Azure AI Search 和 Azure Functions。此外，它還與 Azure AI Foundry 深度集成。

對於 AutoGen 和 Semantic Kernel，你也可以集成 Azure 服務，但可能需要從代碼中調用 Azure 服務。另一種集成方式是使用 Azure SDK 從你的代理中與 Azure 服務交互。此外，如前所述，你可以使用 Azure AI Agent Service 作為 AutoGen 或 Semantic Kernel 中構建的代理的協調器，這樣可以輕鬆訪問 Azure 生態系統。

### 還有更多關於 AI Agent 框架的問題嗎？

加入 [Azure AI Foundry Discord](https://aka.ms/ai-agents/discord)，與其他學習者交流，參加辦公時間，並獲得有關 AI Agent 的問題解答。

## 參考資料

- 

## 上一課

[AI Agent 和使用場景介紹](../01-intro-to-ai-agents/README.md)

## 下一課

[理解代理設計模式](../03-agentic-design-patterns/README.md)

---

**免責聲明**：  
本文件使用 AI 翻譯服務 [Co-op Translator](https://github.com/Azure/co-op-translator) 進行翻譯。我們致力於提供準確的翻譯，但請注意，自動翻譯可能包含錯誤或不準確之處。應以原始語言的文件作為權威來源。對於關鍵資訊，建議尋求專業人工翻譯。我們對因使用此翻譯而產生的任何誤解或錯誤解讀概不負責。