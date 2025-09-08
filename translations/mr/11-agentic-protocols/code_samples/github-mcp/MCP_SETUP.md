<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "c4be907703b836d1a1c360db20da4de9",
  "translation_date": "2025-08-29T11:05:40+00:00",
  "source_file": "11-agentic-protocols/code_samples/github-mcp/MCP_SETUP.md",
  "language_code": "mr"
}
-->
# MCP Server Integration Guide

## पूर्वअट
- Node.js स्थापित (आवृत्ती 14 किंवा त्याहून अधिक)
- npm पॅकेज मॅनेजर
- आवश्यक dependencies असलेले Python वातावरण

## सेटअप चरण

1. **MCP Server पॅकेज स्थापित करा**
   ```bash
   npm install -g @modelcontextprotocol/server-github
   ```

2. **MCP Server सुरू करा**
   ```bash
   npx @modelcontextprotocol/server-github
   ```  
   सर्व्हर सुरू होईल आणि एक कनेक्शन URL प्रदर्शित करेल.

3. **कनेक्शन सत्यापित करा**
   - Chainlit इंटरफेसमध्ये प्लग आयकॉन (🔌) शोधा  
   - प्लग आयकॉनच्या शेजारी एक संख्या (1) दिसली पाहिजे, जी यशस्वी कनेक्शन दर्शवते  
   - कन्सोलमध्ये हे दिसले पाहिजे: "GitHub plugin setup completed successfully" (इतर स्टेटस लाइन्ससह)

## समस्या निवारण

### सामान्य समस्या

1. **पोर्ट संघर्ष**
   ```bash
   Error: listen EADDRINUSE: address already in use
   ```  
   उपाय: पोर्ट बदलण्यासाठी वापरा:  
   ```bash
   npx @modelcontextprotocol/server-github --port 3001
   ```

2. **प्रमाणीकरण समस्या**
   - GitHub credentials योग्यरित्या कॉन्फिगर केले आहेत याची खात्री करा  
   - .env फाइलमध्ये आवश्यक टोकन्स आहेत याची तपासणी करा  
   - GitHub API ऍक्सेस सत्यापित करा  

3. **कनेक्शन अयशस्वी**
   - सर्व्हर अपेक्षित पोर्टवर चालू आहे याची खात्री करा  
   - फायरवॉल सेटिंग्ज तपासा  
   - Python वातावरणात आवश्यक पॅकेजेस आहेत याची खात्री करा  

## कनेक्शन सत्यापन

तुमचा MCP सर्व्हर योग्यरित्या कनेक्ट झाला आहे जेव्हा:  
1. कन्सोलमध्ये "GitHub plugin setup completed successfully" दिसते  
2. कनेक्शन लॉग्समध्ये "✓ MCP Connection Status: Active" दिसते  
3. GitHub कमांड्स चॅट इंटरफेसमध्ये कार्य करतात  

## पर्यावरणीय व्हेरिएबल्स

तुमच्या .env फाइलमध्ये आवश्यक:  
```
GITHUB_TOKEN=your_github_token
MCP_SERVER_PORT=3000  # Optional, default is 3000
```

## कनेक्शन चाचणी

चॅटमध्ये हा चाचणी संदेश पाठवा:  
```
Show me the repositories for username: [GitHub Username]
```  
यशस्वी प्रतिसादात रेपॉझिटरी माहिती दिसेल.  

---

**अस्वीकरण**:  
हा दस्तऐवज AI भाषांतर सेवा [Co-op Translator](https://github.com/Azure/co-op-translator) चा वापर करून भाषांतरित करण्यात आला आहे. आम्ही अचूकतेसाठी प्रयत्नशील असलो तरी, कृपया लक्षात घ्या की स्वयंचलित भाषांतरांमध्ये त्रुटी किंवा अचूकतेचा अभाव असू शकतो. मूळ भाषेतील दस्तऐवज हा अधिकृत स्रोत मानला जावा. महत्त्वाच्या माहितीसाठी व्यावसायिक मानवी भाषांतराची शिफारस केली जाते. या भाषांतराचा वापर केल्यामुळे उद्भवणाऱ्या कोणत्याही गैरसमज किंवा चुकीच्या अर्थासाठी आम्ही जबाबदार राहणार नाही.