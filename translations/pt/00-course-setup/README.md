<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "c55b973b1562abf5aadf6a4028265ac5",
  "translation_date": "2025-08-30T14:12:07+00:00",
  "source_file": "00-course-setup/README.md",
  "language_code": "pt"
}
-->
# Configuração do Curso

## Introdução

Esta lição abordará como executar os exemplos de código deste curso.

## Junte-se a Outros Estudantes e Obtenha Ajuda

Antes de começar a clonar o seu repositório, junte-se ao [canal do Discord AI Agents For Beginners](https://aka.ms/ai-agents/discord) para obter ajuda com a configuração, esclarecer dúvidas sobre o curso ou conectar-se com outros estudantes.

## Clone ou Faça um Fork deste Repositório

Para começar, clone ou faça um fork do repositório GitHub. Isso criará a sua própria versão do material do curso, permitindo que você execute, teste e ajuste o código!

Isso pode ser feito clicando no link para 

Você deve agora ter a sua própria versão forked deste curso no seguinte link:

![Forked Repo](../../../translated_images/forked-repo.33f27ca1901baa6a5e13ec3eb1f0ddd3a44d936d91cc8cfb19bfdb9688bd2c3d.pt.png)

## Executando o Código

Este curso oferece uma série de Jupyter Notebooks que você pode executar para obter experiência prática na construção de Agentes de IA.

Os exemplos de código utilizam:

**Requer Conta GitHub - Gratuita**:

1) Semantic Kernel Agent Framework + GitHub Models Marketplace. Identificado como (semantic-kernel.ipynb)  
2) AutoGen Framework + GitHub Models Marketplace. Identificado como (autogen.ipynb)  

**Requer Subscrição Azure**:  
3) Azure AI Foundry + Azure AI Agent Service. Identificado como (azureaiagent.ipynb)  

Recomendamos que experimente os três tipos de exemplos para descobrir qual funciona melhor para você.

A opção escolhida determinará quais etapas de configuração você precisará seguir abaixo:

## Requisitos

- Python 3.12+  
  - **NOTA**: Se não tiver o Python 3.12 instalado, certifique-se de instalá-lo. Depois, crie o seu ambiente virtual (venv) usando python3.12 para garantir que as versões corretas sejam instaladas a partir do ficheiro requirements.txt.  
- Conta GitHub - Para acesso ao GitHub Models Marketplace  
- Subscrição Azure - Para acesso ao Azure AI Foundry  
- Conta Azure AI Foundry - Para acesso ao Azure AI Agent Service  

Incluímos um ficheiro `requirements.txt` na raiz deste repositório que contém todos os pacotes Python necessários para executar os exemplos de código.

Pode instalá-los executando o seguinte comando no terminal na raiz do repositório:

```bash
pip install -r requirements.txt
```  
Recomendamos criar um ambiente virtual Python para evitar conflitos e problemas.

## Configuração do VSCode

Certifique-se de que está a usar a versão correta do Python no VSCode.

![image](https://github.com/user-attachments/assets/a85e776c-2edb-4331-ae5b-6bfdfb98ee0e)

## Configuração para Exemplos usando GitHub Models

### Passo 1: Recupere o Seu GitHub Personal Access Token (PAT)

Este curso utiliza o GitHub Models Marketplace, que oferece acesso gratuito a Modelos de Linguagem de Grande Escala (LLMs) que você usará para construir Agentes de IA.

Para usar os modelos do GitHub, será necessário criar um [GitHub Personal Access Token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens).

Isso pode ser feito na sua conta GitHub.

Por favor, siga o [Princípio do Menor Privilégio](https://docs.github.com/en/get-started/learning-to-code/storing-your-secrets-safely) ao criar o seu token. Isso significa que deve conceder ao token apenas as permissões necessárias para executar os exemplos de código deste curso.

1. Selecione a opção `Fine-grained tokens` no lado esquerdo do ecrã, navegando até **Developer settings**  
   ![](../../../translated_images/profile_developer_settings.410a859fe749c755c859d414294c5908e307222b2c61819c3203bbeed4470e25.pt.png)

   Em seguida, selecione `Generate new token`.  

   ![Generate Token](../../../translated_images/fga_new_token.1c1a234afe202ab37483944a291ee80c1868e1e78082fd6bd4180fea5d5a15b4.pt.png)

2. Insira um nome descritivo para o seu token que reflita o seu propósito, facilitando a identificação mais tarde.

    🔐 Recomendação de Duração do Token  

    Duração recomendada: 30 dias  
    Para uma postura mais segura, pode optar por um período mais curto—como 7 dias 🛡️  
    É uma ótima forma de definir um objetivo pessoal e concluir o curso enquanto mantém o seu ritmo de aprendizagem 🚀.  

    ![Token Name and Expiration](../../../translated_images/token-name-expiry-date.a095fb0de63868640a4c82d6b1bbc92b482930a663917a5983a3c7cd1ef86b77.pt.png)

3. Limite o escopo do token ao seu fork deste repositório.

    ![Limit scope to fork repository](../../../translated_images/token_repository_limit.924ade5e11d9d8bb6cd21293987e4579dea860e2ba66d607fb46e49524d53644.pt.png)

4. Restrinja as permissões do token: Sob **Permissions**, clique no separador **Account** e depois no botão "+ Add permissions". Aparecerá um menu suspenso. Pesquise por **Models** e marque a caixa correspondente.  
    ![Add Models Permission](../../../translated_images/add_models_permissions.c0c44ed8b40fc143dc87792da9097d715b7de938354e8f771d65416ecc7816b8.pt.png)

5. Verifique as permissões necessárias antes de gerar o token. ![Verify Permissions](../../../translated_images/verify_permissions.06bd9e43987a8b219f171bbcf519e45ababae35b844f5e9757e10afcb619b936.pt.png)

6. Antes de gerar o token, certifique-se de que está pronto para armazená-lo num local seguro, como um cofre de gestor de senhas, pois ele não será exibido novamente após a criação. ![Store Token Securely](../../../translated_images/store_token_securely.08ee2274c6ad6caf3482f1cd1bad7ca3fdca1ce737bc485bfa6499c84297c789.pt.png)

Copie o novo token que acabou de criar. Agora, adicione-o ao ficheiro `.env` incluído neste curso.

### Passo 2: Crie o Seu Ficheiro `.env`

Para criar o ficheiro `.env`, execute o seguinte comando no terminal.

```bash
cp .env.example .env
```

Isso copiará o ficheiro de exemplo e criará um `.env` no seu diretório, onde preencherá os valores das variáveis de ambiente.

Com o token copiado, abra o ficheiro `.env` no seu editor de texto favorito e cole o token no campo `GITHUB_TOKEN`.  
![GitHub Token Field](../../../translated_images/github_token_field.20491ed3224b5f4ab24d10ced7a68c4aba2948fe8999cfc8675edaa16f5e5681.pt.png)

Agora deve ser capaz de executar os exemplos de código deste curso.

## Configuração para Exemplos usando Azure AI Foundry e Azure AI Agent Service

### Passo 1: Recupere o Endpoint do Seu Projeto Azure

Siga os passos para criar um hub e projeto no Azure AI Foundry descritos aqui: [Hub resources overview](https://learn.microsoft.com/en-us/azure/ai-foundry/concepts/ai-resources)

Depois de criar o seu projeto, será necessário recuperar a string de conexão do projeto.

Isso pode ser feito na página **Overview** do seu projeto no portal Azure AI Foundry.

![Project Connection String](../../../translated_images/project-endpoint.8cf04c9975bbfbf18f6447a599550edb052e52264fb7124d04a12e6175e330a5.pt.png)

### Passo 2: Crie o Seu Ficheiro `.env`

Para criar o ficheiro `.env`, execute o seguinte comando no terminal.

```bash
cp .env.example .env
```

Isso copiará o ficheiro de exemplo e criará um `.env` no seu diretório, onde preencherá os valores das variáveis de ambiente.

Com o token copiado, abra o ficheiro `.env` no seu editor de texto favorito e cole o token no campo `PROJECT_ENDPOINT`.

### Passo 3: Inicie Sessão no Azure

Como uma prática recomendada de segurança, utilizaremos a [autenticação sem chave](https://learn.microsoft.com/azure/developer/ai/keyless-connections?tabs=csharp%2Cazure-cli?WT.mc_id=academic-105485-koreyst) para autenticar no Azure OpenAI com o Microsoft Entra ID.

Em seguida, abra um terminal e execute `az login --use-device-code` para iniciar sessão na sua conta Azure.

Depois de iniciar sessão, selecione a sua subscrição no terminal.

## Variáveis de Ambiente Adicionais - Azure Search e Azure OpenAI

Para a lição Agentic RAG - Lição 5 - há exemplos que utilizam Azure Search e Azure OpenAI.

Se quiser executar esses exemplos, será necessário adicionar as seguintes variáveis de ambiente ao ficheiro `.env`:

### Página de Resumo (Projeto)

- `AZURE_SUBSCRIPTION_ID` - Verifique **Project details** na página **Overview** do seu projeto.

- `AZURE_AI_PROJECT_NAME` - Consulte o topo da página **Overview** do seu projeto.

- `AZURE_OPENAI_SERVICE` - Encontre isto no separador **Included capabilities** para **Azure OpenAI Service** na página **Overview**.

### Centro de Gestão

- `AZURE_OPENAI_RESOURCE_GROUP` - Vá para **Project properties** na página **Overview** do **Management Center**.

- `GLOBAL_LLM_SERVICE` - Em **Connected resources**, encontre o nome da conexão **Azure AI Services**. Se não estiver listado, verifique no **Azure portal** sob o seu grupo de recursos o nome do recurso AI Services.

### Página de Modelos + Endpoints

- `AZURE_OPENAI_EMBEDDING_DEPLOYMENT_NAME` - Selecione o seu modelo de embedding (por exemplo, `text-embedding-ada-002`) e anote o **Deployment name** nos detalhes do modelo.

- `AZURE_OPENAI_CHAT_DEPLOYMENT_NAME` - Selecione o seu modelo de chat (por exemplo, `gpt-4o-mini`) e anote o **Deployment name** nos detalhes do modelo.

### Portal Azure

- `AZURE_OPENAI_ENDPOINT` - Procure por **Azure AI services**, clique nele, depois vá para **Resource Management**, **Keys and Endpoint**, desça até "Azure OpenAI endpoints" e copie o que diz "Language APIs".

- `AZURE_OPENAI_API_KEY` - Na mesma tela, copie a CHAVE 1 ou CHAVE 2.

- `AZURE_SEARCH_SERVICE_ENDPOINT` - Encontre o recurso **Azure AI Search**, clique nele e veja **Overview**.

- `AZURE_SEARCH_API_KEY` - Depois vá para **Settings** e depois **Keys** para copiar a chave de administrador primária ou secundária.

### Página Externa

- `AZURE_OPENAI_API_VERSION` - Visite a página [API version lifecycle](https://learn.microsoft.com/en-us/azure/ai-services/openai/api-version-deprecation#latest-ga-api-release) sob **Latest GA API release**.

### Configuração de autenticação sem chave

Em vez de codificar as suas credenciais, utilizaremos uma conexão sem chave com o Azure OpenAI. Para isso, importaremos `DefaultAzureCredential` e mais tarde chamaremos a função `DefaultAzureCredential` para obter a credencial.

```python
from azure.identity import DefaultAzureCredential, InteractiveBrowserCredential
```

## Com Dificuldades?

Se tiver algum problema ao executar esta configuração, entre no nosso 

ou 

## Próxima Lição

Agora está pronto para executar o código deste curso. Boa aprendizagem sobre o mundo dos Agentes de IA!

[Introdução aos Agentes de IA e Casos de Uso de Agentes](../01-intro-to-ai-agents/README.md)

---

**Aviso Legal**:  
Este documento foi traduzido utilizando o serviço de tradução por IA [Co-op Translator](https://github.com/Azure/co-op-translator). Embora nos esforcemos para garantir a precisão, esteja ciente de que traduções automáticas podem conter erros ou imprecisões. O documento original no seu idioma nativo deve ser considerado a fonte oficial. Para informações críticas, recomenda-se uma tradução profissional realizada por humanos. Não nos responsabilizamos por quaisquer mal-entendidos ou interpretações incorretas resultantes do uso desta tradução.