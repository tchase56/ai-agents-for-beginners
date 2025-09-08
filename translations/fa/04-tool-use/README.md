<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "4a5ccc4ad1dba85fbc2087cf3b986544",
  "translation_date": "2025-08-30T13:36:57+00:00",
  "source_file": "04-tool-use/README.md",
  "language_code": "fa"
}
-->
[![چگونه عوامل هوش مصنوعی خوب طراحی کنیم](../../../translated_images/lesson-4-thumbnail.546162853cb3daffd64edd92014f274103f76360dfb39fc6e6ee399494da38fd.fa.png)](https://youtu.be/vieRiPRx-gI?si=cEZ8ApnT6Sus9rhn)

> _(برای مشاهده ویدئوی این درس روی تصویر بالا کلیک کنید)_

# الگوی طراحی استفاده از ابزار

ابزارها جالب هستند زیرا به عوامل هوش مصنوعی اجازه می‌دهند تا دامنه وسیع‌تری از قابلیت‌ها داشته باشند. به جای اینکه عامل تنها مجموعه محدودی از اقدامات را انجام دهد، با افزودن یک ابزار، عامل اکنون می‌تواند طیف گسترده‌ای از اقدامات را انجام دهد. در این فصل، به الگوی طراحی استفاده از ابزار می‌پردازیم که توضیح می‌دهد چگونه عوامل هوش مصنوعی می‌توانند از ابزارهای خاص برای دستیابی به اهداف خود استفاده کنند.

## مقدمه

در این درس، به دنبال پاسخ به سوالات زیر هستیم:

- الگوی طراحی استفاده از ابزار چیست؟
- موارد استفاده‌ای که می‌توان آن را به کار برد کدامند؟
- عناصر/بلوک‌های سازنده مورد نیاز برای پیاده‌سازی این الگوی طراحی چیست؟
- ملاحظات ویژه برای استفاده از الگوی طراحی استفاده از ابزار برای ساخت عوامل هوش مصنوعی قابل اعتماد چیست؟

## اهداف یادگیری

پس از اتمام این درس، شما قادر خواهید بود:

- الگوی طراحی استفاده از ابزار و هدف آن را تعریف کنید.
- موارد استفاده‌ای که این الگوی طراحی در آن‌ها کاربرد دارد را شناسایی کنید.
- عناصر کلیدی مورد نیاز برای پیاده‌سازی این الگوی طراحی را درک کنید.
- ملاحظات لازم برای اطمینان از اعتمادپذیری عوامل هوش مصنوعی با استفاده از این الگوی طراحی را تشخیص دهید.

## الگوی طراحی استفاده از ابزار چیست؟

**الگوی طراحی استفاده از ابزار** بر توانمندسازی مدل‌های زبانی بزرگ (LLM) برای تعامل با ابزارهای خارجی به منظور دستیابی به اهداف خاص تمرکز دارد. ابزارها کدهایی هستند که می‌توانند توسط یک عامل اجرا شوند تا اقدامات خاصی انجام دهند. یک ابزار می‌تواند یک تابع ساده مانند یک ماشین حساب باشد یا یک فراخوانی API به یک سرویس شخص ثالث مانند جستجوی قیمت سهام یا پیش‌بینی آب‌وهوا. در زمینه عوامل هوش مصنوعی، ابزارها به گونه‌ای طراحی شده‌اند که توسط عوامل در پاسخ به **فراخوانی‌های تابع تولید شده توسط مدل** اجرا شوند.

## موارد استفاده‌ای که می‌توان آن را به کار برد کدامند؟

عوامل هوش مصنوعی می‌توانند از ابزارها برای انجام وظایف پیچیده، بازیابی اطلاعات یا تصمیم‌گیری استفاده کنند. الگوی طراحی استفاده از ابزار اغلب در سناریوهایی که نیاز به تعامل پویا با سیستم‌های خارجی مانند پایگاه‌های داده، خدمات وب یا مفسرهای کد دارند، استفاده می‌شود. این قابلیت برای موارد استفاده مختلفی مفید است، از جمله:

- **بازیابی اطلاعات پویا:** عوامل می‌توانند APIها یا پایگاه‌های داده خارجی را برای دریافت داده‌های به‌روز جستجو کنند (مثلاً جستجو در یک پایگاه داده SQLite برای تحلیل داده‌ها، دریافت قیمت سهام یا اطلاعات آب‌وهوا).
- **اجرای کد و تفسیر:** عوامل می‌توانند کد یا اسکریپت‌ها را برای حل مسائل ریاضی، تولید گزارش‌ها یا انجام شبیه‌سازی‌ها اجرا کنند.
- **اتوماسیون فرآیندها:** خودکارسازی فرآیندهای تکراری یا چندمرحله‌ای با ادغام ابزارهایی مانند زمان‌بندهای وظیفه، خدمات ایمیل یا خطوط لوله داده.
- **پشتیبانی مشتری:** عوامل می‌توانند با سیستم‌های مدیریت ارتباط با مشتری (CRM)، پلتفرم‌های تیکتینگ یا پایگاه‌های دانش تعامل داشته باشند تا به سوالات کاربران پاسخ دهند.
- **تولید و ویرایش محتوا:** عوامل می‌توانند از ابزارهایی مانند بررسی‌کننده‌های گرامر، خلاصه‌کننده‌های متن یا ارزیاب‌های ایمنی محتوا برای کمک به وظایف تولید محتوا استفاده کنند.

## عناصر/بلوک‌های سازنده مورد نیاز برای پیاده‌سازی الگوی طراحی استفاده از ابزار چیست؟

این بلوک‌های سازنده به عامل هوش مصنوعی اجازه می‌دهند تا طیف گسترده‌ای از وظایف را انجام دهد. بیایید به عناصر کلیدی مورد نیاز برای پیاده‌سازی الگوی طراحی استفاده از ابزار نگاهی بیندازیم:

- **طرح‌های تابع/ابزار:** تعریفات دقیق ابزارهای موجود، شامل نام تابع، هدف، پارامترهای مورد نیاز و خروجی‌های مورد انتظار. این طرح‌ها به مدل زبانی بزرگ کمک می‌کنند تا بفهمد چه ابزارهایی در دسترس هستند و چگونه درخواست‌های معتبر ایجاد کند.

- **منطق اجرای تابع:** تعیین می‌کند که چگونه و چه زمانی ابزارها بر اساس قصد کاربر و زمینه مکالمه فراخوانی شوند. این ممکن است شامل ماژول‌های برنامه‌ریز، مکانیزم‌های مسیریابی یا جریان‌های شرطی باشد که استفاده از ابزار را به صورت پویا تعیین می‌کنند.

- **سیستم مدیریت پیام:** اجزایی که جریان مکالمه بین ورودی‌های کاربر، پاسخ‌های مدل زبانی بزرگ، فراخوانی‌های ابزار و خروجی‌های ابزار را مدیریت می‌کنند.

- **چارچوب یکپارچه‌سازی ابزار:** زیرساختی که عامل را به ابزارهای مختلف متصل می‌کند، چه این ابزارها توابع ساده باشند یا خدمات خارجی پیچیده.

- **مدیریت خطا و اعتبارسنجی:** مکانیزم‌هایی برای مدیریت شکست‌ها در اجرای ابزار، اعتبارسنجی پارامترها و مدیریت پاسخ‌های غیرمنتظره.

- **مدیریت وضعیت:** پیگیری زمینه مکالمه، تعاملات قبلی با ابزار و داده‌های پایدار برای اطمینان از سازگاری در تعاملات چندمرحله‌ای.

در ادامه، به جزئیات بیشتری درباره فراخوانی تابع/ابزار می‌پردازیم.

### فراخوانی تابع/ابزار

فراخوانی تابع اصلی‌ترین روش برای توانمندسازی مدل‌های زبانی بزرگ (LLM) جهت تعامل با ابزارها است. اغلب اوقات، اصطلاحات "تابع" و "ابزار" به صورت متقابل استفاده می‌شوند زیرا "توابع" (بلوک‌های کد قابل استفاده مجدد) همان "ابزارهایی" هستند که عوامل برای انجام وظایف از آن‌ها استفاده می‌کنند. برای اینکه کد یک تابع فراخوانی شود، مدل زبانی بزرگ باید درخواست کاربر را با توضیحات تابع مقایسه کند. برای این کار، یک طرح شامل توضیحات تمام توابع موجود به مدل زبانی بزرگ ارسال می‌شود. مدل زبانی بزرگ سپس مناسب‌ترین تابع را برای وظیفه انتخاب کرده و نام و آرگومان‌های آن را بازمی‌گرداند. تابع انتخاب‌شده فراخوانی می‌شود، پاسخ آن به مدل زبانی بزرگ ارسال می‌شود و مدل از این اطلاعات برای پاسخ به درخواست کاربر استفاده می‌کند.

برای پیاده‌سازی فراخوانی تابع برای عوامل، توسعه‌دهندگان به موارد زیر نیاز دارند:

1. یک مدل زبانی بزرگ که از فراخوانی تابع پشتیبانی کند
2. یک طرح شامل توضیحات توابع
3. کد هر تابع توصیف‌شده

برای مثال، فرض کنید می‌خواهیم زمان فعلی در یک شهر را دریافت کنیم:

1. **ابتدا یک مدل زبانی بزرگ که از فراخوانی تابع پشتیبانی می‌کند را مقداردهی کنید:**

    همه مدل‌ها از فراخوانی تابع پشتیبانی نمی‌کنند، بنابراین مهم است که بررسی کنید مدل زبانی بزرگی که استفاده می‌کنید این قابلیت را دارد. <a href="https://learn.microsoft.com/azure/ai-services/openai/how-to/function-calling" target="_blank">Azure OpenAI</a> از فراخوانی تابع پشتیبانی می‌کند. می‌توانیم با مقداردهی کلاینت Azure OpenAI شروع کنیم.

    ```python
    # Initialize the Azure OpenAI client
    client = AzureOpenAI(
        azure_endpoint = os.getenv("AZURE_OPENAI_ENDPOINT"), 
        api_key=os.getenv("AZURE_OPENAI_API_KEY"),  
        api_version="2024-05-01-preview"
    )
    ```

1. **یک طرح تابع ایجاد کنید:**

    سپس یک طرح JSON تعریف می‌کنیم که شامل نام تابع، توضیحی درباره کاری که تابع انجام می‌دهد و نام‌ها و توضیحات پارامترهای تابع است. این طرح را به همراه درخواست کاربر برای یافتن زمان در سانفرانسیسکو به کلاینتی که قبلاً ایجاد شده ارسال می‌کنیم. نکته مهم این است که **فراخوانی ابزار** چیزی است که بازمی‌گردد، نه پاسخ نهایی به سوال. همان‌طور که قبلاً ذکر شد، مدل زبانی بزرگ نام تابعی را که برای وظیفه انتخاب کرده و آرگومان‌هایی که به آن ارسال می‌شود بازمی‌گرداند.

    ```python
    # Function description for the model to read
    tools = [
        {
            "type": "function",
            "function": {
                "name": "get_current_time",
                "description": "Get the current time in a given location",
                "parameters": {
                    "type": "object",
                    "properties": {
                        "location": {
                            "type": "string",
                            "description": "The city name, e.g. San Francisco",
                        },
                    },
                    "required": ["location"],
                },
            }
        }
    ]
    ```
   
    ```python
  
    # Initial user message
    messages = [{"role": "user", "content": "What's the current time in San Francisco"}] 
  
    # First API call: Ask the model to use the function
      response = client.chat.completions.create(
          model=deployment_name,
          messages=messages,
          tools=tools,
          tool_choice="auto",
      )
  
      # Process the model's response
      response_message = response.choices[0].message
      messages.append(response_message)
  
      print("Model's response:")  

      print(response_message)
  
    ```

    ```bash
    Model's response:
    ChatCompletionMessage(content=None, role='assistant', function_call=None, tool_calls=[ChatCompletionMessageToolCall(id='call_pOsKdUlqvdyttYB67MOj434b', function=Function(arguments='{"location":"San Francisco"}', name='get_current_time'), type='function')])
    ```
  
1. **کد تابع مورد نیاز برای انجام وظیفه:**

    اکنون که مدل زبانی بزرگ انتخاب کرده کدام تابع باید اجرا شود، کدی که وظیفه را انجام می‌دهد باید پیاده‌سازی و اجرا شود. می‌توانیم کدی برای دریافت زمان فعلی در پایتون پیاده‌سازی کنیم. همچنین باید کدی برای استخراج نام و آرگومان‌ها از response_message بنویسیم تا نتیجه نهایی را دریافت کنیم.

    ```python
      def get_current_time(location):
        """Get the current time for a given location"""
        print(f"get_current_time called with location: {location}")  
        location_lower = location.lower()
        
        for key, timezone in TIMEZONE_DATA.items():
            if key in location_lower:
                print(f"Timezone found for {key}")  
                current_time = datetime.now(ZoneInfo(timezone)).strftime("%I:%M %p")
                return json.dumps({
                    "location": location,
                    "current_time": current_time
                })
      
        print(f"No timezone data found for {location_lower}")  
        return json.dumps({"location": location, "current_time": "unknown"})
    ```

     ```python
     # Handle function calls
      if response_message.tool_calls:
          for tool_call in response_message.tool_calls:
              if tool_call.function.name == "get_current_time":
     
                  function_args = json.loads(tool_call.function.arguments)
     
                  time_response = get_current_time(
                      location=function_args.get("location")
                  )
     
                  messages.append({
                      "tool_call_id": tool_call.id,
                      "role": "tool",
                      "name": "get_current_time",
                      "content": time_response,
                  })
      else:
          print("No tool calls were made by the model.")  
  
      # Second API call: Get the final response from the model
      final_response = client.chat.completions.create(
          model=deployment_name,
          messages=messages,
      )
  
      return final_response.choices[0].message.content
     ```

     ```bash
      get_current_time called with location: San Francisco
      Timezone found for san francisco
      The current time in San Francisco is 09:24 AM.
     ```

فراخوانی تابع هسته اصلی اکثر طراحی‌های استفاده از ابزار توسط عوامل است، اما پیاده‌سازی آن از ابتدا گاهی اوقات می‌تواند چالش‌برانگیز باشد. همان‌طور که در [درس ۲](../../../02-explore-agentic-frameworks) یاد گرفتیم، چارچوب‌های عاملیک به ما بلوک‌های سازنده از پیش ساخته‌شده‌ای برای پیاده‌سازی استفاده از ابزار ارائه می‌دهند.

## مثال‌هایی از استفاده از ابزار با چارچوب‌های عاملیک

در اینجا چند مثال از نحوه پیاده‌سازی الگوی طراحی استفاده از ابزار با استفاده از چارچوب‌های عاملیک مختلف آورده شده است:

### Semantic Kernel

<a href="https://learn.microsoft.com/azure/ai-services/agents/overview" target="_blank">Semantic Kernel</a> یک چارچوب هوش مصنوعی متن‌باز برای توسعه‌دهندگان .NET، پایتون و جاوا است که با مدل‌های زبانی بزرگ (LLM) کار می‌کنند. این چارچوب فرآیند استفاده از فراخوانی تابع را با توصیف خودکار توابع و پارامترهای آن‌ها برای مدل از طریق فرآیندی به نام <a href="https://learn.microsoft.com/semantic-kernel/concepts/ai-services/chat-completion/function-calling/?pivots=programming-language-python#1-serializing-the-functions" target="_blank">سریال‌سازی</a> ساده می‌کند. همچنین ارتباطات بین مدل و کد شما را مدیریت می‌کند. یکی دیگر از مزایای استفاده از یک چارچوب عاملیک مانند Semantic Kernel این است که به شما امکان دسترسی به ابزارهای از پیش ساخته‌شده مانند <a href="https://github.com/microsoft/semantic-kernel/blob/main/python/samples/getting_started_with_agents/openai_assistant/step4_assistant_tool_file_search.py" target="_blank">جستجوی فایل</a> و <a href="https://github.com/microsoft/semantic-kernel/blob/main/python/samples/getting_started_with_agents/openai_assistant/step3_assistant_tool_code_interpreter.py" target="_blank">مفسر کد</a> را می‌دهد.

نمودار زیر فرآیند فراخوانی تابع با Semantic Kernel را نشان می‌دهد:

![فراخوانی تابع](../../../translated_images/functioncalling-diagram.a84006fc287f60140cc0a484ff399acd25f69553ea05186981ac4d5155f9c2f6.fa.png)

در Semantic Kernel، توابع/ابزارها <a href="https://learn.microsoft.com/semantic-kernel/concepts/plugins/?pivots=programming-language-python" target="_blank">پلاگین</a> نامیده می‌شوند. می‌توانیم تابع `get_current_time` که قبلاً دیدیم را با تبدیل آن به یک کلاس حاوی تابع به یک پلاگین تبدیل کنیم. همچنین می‌توانیم دکوراتور `kernel_function` را وارد کنیم که توضیحات تابع را دریافت می‌کند. هنگامی که یک کرنل با پلاگین GetCurrentTimePlugin ایجاد می‌کنید، کرنل به طور خودکار تابع و پارامترهای آن را سریال‌سازی می‌کند و در این فرآیند طرحی برای ارسال به مدل ایجاد می‌کند.

```python
from semantic_kernel.functions import kernel_function

class GetCurrentTimePlugin:
    async def __init__(self, location):
        self.location = location

    @kernel_function(
        description="Get the current time for a given location"
    )
    def get_current_time(location: str = ""):
        ...

```

```python 
from semantic_kernel import Kernel

# Create the kernel
kernel = Kernel()

# Create the plugin
get_current_time_plugin = GetCurrentTimePlugin(location)

# Add the plugin to the kernel
kernel.add_plugin(get_current_time_plugin)
```
  
### سرویس عامل Azure AI

<a href="https://learn.microsoft.com/azure/ai-services/agents/overview" target="_blank">سرویس عامل Azure AI</a> یک چارچوب عاملیک جدیدتر است که برای توانمندسازی توسعه‌دهندگان برای ساخت، استقرار و مقیاس‌بندی عوامل هوش مصنوعی با کیفیت بالا و قابل توسعه بدون نیاز به مدیریت منابع محاسباتی و ذخیره‌سازی زیرین طراحی شده است. این سرویس به ویژه برای برنامه‌های سازمانی مفید است زیرا یک سرویس کاملاً مدیریت‌شده با امنیت در سطح سازمانی است.

در مقایسه با توسعه با استفاده از API مدل زبانی بزرگ به طور مستقیم، سرویس عامل Azure AI مزایایی ارائه می‌دهد، از جمله:

- فراخوانی ابزار خودکار – نیازی به تجزیه یک فراخوانی ابزار، اجرای ابزار و مدیریت پاسخ نیست؛ همه این‌ها اکنون در سمت سرور انجام می‌شود.
- مدیریت داده‌های امن – به جای مدیریت وضعیت مکالمه خود، می‌توانید به رشته‌ها برای ذخیره تمام اطلاعات مورد نیاز خود تکیه کنید.
- ابزارهای آماده استفاده – ابزارهایی که می‌توانید برای تعامل با منابع داده خود استفاده کنید، مانند Bing، Azure AI Search و Azure Functions.

ابزارهای موجود در سرویس عامل Azure AI را می‌توان به دو دسته تقسیم کرد:

1. ابزارهای دانش:
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/bing-grounding?tabs=python&pivots=overview" target="_blank">پایه‌گذاری با جستجوی Bing</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/file-search?tabs=python&pivots=overview" target="_blank">جستجوی فایل</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/azure-ai-search?tabs=azurecli%2Cpython&pivots=overview-azure-ai-search" target="_blank">Azure AI Search</a>

2. ابزارهای عملیاتی:
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/function-calling?tabs=python&pivots=overview" target="_blank">فراخوانی تابع</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/code-interpreter?tabs=python&pivots=overview" target="_blank">مفسر کد</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/openapi-spec?tabs=python&pivots=overview" target="_blank">ابزارهای تعریف‌شده توسط OpenAI</a>
    - <a href="https://learn.microsoft.com/azure/ai-services/agents/how-to/tools/azure-functions?pivots=overview" target="_blank">Azure Functions</a>

سرویس عامل به ما این امکان را می‌دهد که بتوانیم از این ابزارها به صورت یک `toolset` استفاده کنیم. همچنین از `threads` استفاده می‌کند که تاریخچه پیام‌ها از یک مکالمه خاص را پیگیری می‌کنند.

تصور کنید شما یک نماینده فروش در شرکتی به نام Contoso هستید. می‌خواهید یک عامل مکالمه‌ای توسعه دهید که بتواند به سوالات مربوط به داده‌های فروش شما پاسخ دهد.

تصویر زیر نشان می‌دهد که چگونه می‌توانید از سرویس عامل Azure AI برای تحلیل داده‌های فروش خود استفاده کنید:

![سرویس عامل در عمل](../../../translated_images/agent-service-in-action.34fb465c9a84659edd3003f8cb62d6b366b310a09b37c44e32535021fbb5c93f.fa.jpg)

برای استفاده از هر یک از این ابزارها با سرویس، می‌توانیم یک کلاینت ایجاد کرده و یک ابزار یا مجموعه ابزار تعریف کنیم. برای پیاده‌سازی این کار به صورت عملی می‌توانیم از کد پایتون زیر استفاده کنیم. مدل زبانی بزرگ قادر خواهد بود به مجموعه ابزار نگاه کند و بسته به درخواست کاربر تصمیم بگیرد که آیا از تابع کاربر ایجاد‌شده `fetch_sales_data_using_sqlite_query` استفاده کند یا از مفسر کد از پیش ساخته‌شده.

```python 
import os
from azure.ai.projects import AIProjectClient
from azure.identity import DefaultAzureCredential
from fetch_sales_data_functions import fetch_sales_data_using_sqlite_query # fetch_sales_data_using_sqlite_query function which can be found in a fetch_sales_data_functions.py file.
from azure.ai.projects.models import ToolSet, FunctionTool, CodeInterpreterTool

project_client = AIProjectClient.from_connection_string(
    credential=DefaultAzureCredential(),
    conn_str=os.environ["PROJECT_CONNECTION_STRING"],
)

# Initialize function calling agent with the fetch_sales_data_using_sqlite_query function and adding it to the toolset
fetch_data_function = FunctionTool(fetch_sales_data_using_sqlite_query)
toolset = ToolSet()
toolset.add(fetch_data_function)

# Initialize Code Interpreter tool and adding it to the toolset. 
code_interpreter = code_interpreter = CodeInterpreterTool()
toolset = ToolSet()
toolset.add(code_interpreter)

agent = project_client.agents.create_agent(
    model="gpt-4o-mini", name="my-agent", instructions="You are helpful agent", 
    toolset=toolset
)
```

## ملاحظات ویژه برای استفاده از الگوی طراحی استفاده از ابزار برای ساخت عوامل هوش مصنوعی قابل اعتماد چیست؟

یکی از نگرانی‌های رایج در مورد SQL که به صورت پویا توسط مدل‌های زبانی بزرگ تولید می‌شود، امنیت است، به ویژه خطر تزریق SQL یا اقدامات مخرب مانند حذف یا دستکاری پایگاه داده. اگرچه این نگرانی‌ها معتبر هستند، اما می‌توان آن‌ها را با پیکربندی صحیح مجوزهای دسترسی به پایگاه داده به طور مؤثر کاهش داد. برای اکثر پایگاه‌های داده، این شامل پیکربندی پایگاه داده به صورت فقط خواندنی است. برای خدمات پایگاه داده مانند PostgreSQL یا Azure SQL، باید به برنامه یک نقش فقط خواندنی (SELECT) اختصاص داده شود.

اجرای برنامه در یک محیط امن حفاظت بیشتری را فراهم می‌کند. در سناریوهای سازمانی، داده‌ها معمولاً از سیستم‌های عملیاتی استخراج و به یک پایگاه داده فقط خواندنی یا انبار داده با یک طرح کاربرپسند تبدیل می‌شوند. این رویکرد اطمینان می‌دهد که داده‌ها امن هستند، برای عملکرد و دسترسی بهینه شده‌اند و برنامه دسترسی محدود و فقط خواندنی دارد.

### سوالات بیشتری درباره الگوی طراحی استفاده از ابزار دارید؟
به [دیسکورد Azure AI Foundry](https://aka.ms/ai-agents/discord) بپیوندید تا با دیگر یادگیرندگان ملاقات کنید، در ساعات اداری شرکت کنید و پاسخ سوالات خود درباره عوامل هوش مصنوعی را دریافت کنید.

## منابع اضافی

## درس قبلی

[درک الگوهای طراحی عامل‌محور](../03-agentic-design-patterns/README.md)

## درس بعدی

[عامل‌محور RAG](../05-agentic-rag/README.md)

---

**سلب مسئولیت**:  
این سند با استفاده از سرویس ترجمه هوش مصنوعی [Co-op Translator](https://github.com/Azure/co-op-translator) ترجمه شده است. در حالی که ما تلاش می‌کنیم دقت را حفظ کنیم، لطفاً توجه داشته باشید که ترجمه‌های خودکار ممکن است شامل خطاها یا نادقتی‌ها باشند. سند اصلی به زبان اصلی آن باید به عنوان منبع معتبر در نظر گرفته شود. برای اطلاعات حساس، ترجمه حرفه‌ای انسانی توصیه می‌شود. ما هیچ مسئولیتی در قبال سوءتفاهم‌ها یا تفسیرهای نادرست ناشی از استفاده از این ترجمه نداریم.