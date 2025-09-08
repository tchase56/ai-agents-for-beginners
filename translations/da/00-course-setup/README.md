<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "c55b973b1562abf5aadf6a4028265ac5",
  "translation_date": "2025-08-29T15:39:35+00:00",
  "source_file": "00-course-setup/README.md",
  "language_code": "da"
}
-->
# Kursusopsætning

## Introduktion

Denne lektion dækker, hvordan du kan køre kodeeksemplerne fra dette kursus.

## Deltag med andre kursister og få hjælp

Før du begynder at klone dit repo, skal du tilmelde dig [AI Agents For Beginners Discord-kanalen](https://aka.ms/ai-agents/discord) for at få hjælp til opsætning, stille spørgsmål om kurset eller komme i kontakt med andre kursister.

## Klon eller fork dette repo

For at komme i gang skal du klone eller fork GitHub-repositoriet. Dette vil give dig din egen version af kursusmaterialet, så du kan køre, teste og tilpasse koden!

Dette kan gøres ved at klikke på linket til

Du bør nu have din egen forkede version af dette kursus på følgende link:

![Forked Repo](../../../translated_images/forked-repo.33f27ca1901baa6a5e13ec3eb1f0ddd3a44d936d91cc8cfb19bfdb9688bd2c3d.da.png)

## Kør koden

Dette kursus tilbyder en række Jupyter Notebooks, som du kan køre for at få praktisk erfaring med at bygge AI-agenter.

Kodeeksemplerne bruger enten:

**Kræver GitHub-konto - Gratis**:

1) Semantic Kernel Agent Framework + GitHub Models Marketplace. Markeret som (semantic-kernel.ipynb)
2) AutoGen Framework + GitHub Models Marketplace. Markeret som (autogen.ipynb)

**Kræver Azure-abonnement**:
3) Azure AI Foundry + Azure AI Agent Service. Markeret som (azureaiagent.ipynb)

Vi opfordrer dig til at prøve alle tre typer eksempler for at se, hvilken der fungerer bedst for dig.

Uanset hvilken mulighed du vælger, vil det afgøre, hvilke opsætningsinstruktioner du skal følge nedenfor:

## Krav

- Python 3.12+
  - **NOTE**: Hvis du ikke har Python 3.12 installeret, skal du sørge for at installere det. Opret derefter din venv ved hjælp af python3.12 for at sikre, at de korrekte versioner installeres fra requirements.txt-filen.
- En GitHub-konto - For adgang til GitHub Models Marketplace
- Azure-abonnement - For adgang til Azure AI Foundry
- Azure AI Foundry-konto - For adgang til Azure AI Agent Service

Vi har inkluderet en `requirements.txt`-fil i roden af dette repository, som indeholder alle de nødvendige Python-pakker for at køre kodeeksemplerne.

Du kan installere dem ved at køre følgende kommando i din terminal i roden af repositoriet:

```bash
pip install -r requirements.txt
```
Vi anbefaler at oprette et Python-virtuelt miljø for at undgå konflikter og problemer.

## Opsætning af VSCode
Sørg for, at du bruger den korrekte version af Python i VSCode.

![image](https://github.com/user-attachments/assets/a85e776c-2edb-4331-ae5b-6bfdfb98ee0e)

## Opsætning til eksempler med GitHub-modeller

### Trin 1: Hent din GitHub Personal Access Token (PAT)

Dette kursus benytter GitHub Models Marketplace, som giver gratis adgang til Large Language Models (LLMs), som du vil bruge til at bygge AI-agenter.

For at bruge GitHub-modellerne skal du oprette en [GitHub Personal Access Token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens).

Dette kan gøres ved at gå til din GitHub-konto.

Følg venligst [Principle of Least Privilege](https://docs.github.com/en/get-started/learning-to-code/storing-your-secrets-safely), når du opretter din token. Det betyder, at du kun skal give token de tilladelser, der er nødvendige for at køre kodeeksemplerne i dette kursus.

1. Vælg `Fine-grained tokens`-muligheden i venstre side af skærmen ved at navigere til **Developer settings**.
   ![](../../../translated_images/profile_developer_settings.410a859fe749c755c859d414294c5908e307222b2c61819c3203bbeed4470e25.da.png)

    Vælg derefter `Generate new token`.

    ![Generate Token](../../../translated_images/fga_new_token.1c1a234afe202ab37483944a291ee80c1868e1e78082fd6bd4180fea5d5a15b4.da.png)

2. Indtast et beskrivende navn til din token, der afspejler dens formål, så den er nem at identificere senere.

    🔐 Anbefaling for token-varighed

    Anbefalet varighed: 30 dage  
    For en mere sikker tilgang kan du vælge en kortere periode—såsom 7 dage 🛡️  
    Det er en god måde at sætte et personligt mål og gennemføre kurset, mens din læringsmotivation er høj 🚀.

    ![Token Name and Expiration](../../../translated_images/token-name-expiry-date.a095fb0de63868640a4c82d6b1bbc92b482930a663917a5983a3c7cd1ef86b77.da.png)

3. Begræns tokenens rækkevidde til din fork af dette repository.

    ![Limit scope to fork repository](../../../translated_images/token_repository_limit.924ade5e11d9d8bb6cd21293987e4579dea860e2ba66d607fb46e49524d53644.da.png)

4. Begræns tokenens tilladelser: Under **Permissions**, klik på **Account**-fanen, og klik på knappen "+ Add permissions". En dropdown-menu vil dukke op. Søg efter **Models** og marker boksen for det.
    ![Add Models Permission](../../../translated_images/add_models_permissions.c0c44ed8b40fc143dc87792da9097d715b7de938354e8f771d65416ecc7816b8.da.png)

5. Bekræft de nødvendige tilladelser, før du genererer token. ![Verify Permissions](../../../translated_images/verify_permissions.06bd9e43987a8b219f171bbcf519e45ababae35b844f5e9757e10afcb619b936.da.png)

6. Før du genererer token, skal du sørge for at gemme den på et sikkert sted som en password manager, da den ikke vil blive vist igen efter oprettelsen. ![Store Token Securely](../../../translated_images/store_token_securely.08ee2274c6ad6caf3482f1cd1bad7ca3fdca1ce737bc485bfa6499c84297c789.da.png)

Kopiér din nye token, som du lige har oprettet. Du skal nu tilføje denne til din `.env`-fil, der er inkluderet i dette kursus.

### Trin 2: Opret din `.env`-fil

For at oprette din `.env`-fil skal du køre følgende kommando i din terminal.

```bash
cp .env.example .env
```

Dette vil kopiere eksempel-filen og oprette en `.env` i din mappe, hvor du kan udfylde værdierne for miljøvariablerne.

Med din token kopieret, skal du åbne `.env`-filen i din foretrukne teksteditor og indsætte din token i `GITHUB_TOKEN`-feltet.  
![GitHub Token Field](../../../translated_images/github_token_field.20491ed3224b5f4ab24d10ced7a68c4aba2948fe8999cfc8675edaa16f5e5681.da.png)

Du bør nu kunne køre kodeeksemplerne fra dette kursus.

## Opsætning til eksempler med Azure AI Foundry og Azure AI Agent Service

### Trin 1: Hent din Azure-projekt-endpoint

Følg trinnene til at oprette en hub og et projekt i Azure AI Foundry, som beskrevet her: [Hub resources overview](https://learn.microsoft.com/en-us/azure/ai-foundry/concepts/ai-resources)

Når du har oprettet dit projekt, skal du hente forbindelsesstrengen for dit projekt.

Dette kan gøres ved at gå til **Overview**-siden for dit projekt i Azure AI Foundry-portalen.

![Project Connection String](../../../translated_images/project-endpoint.8cf04c9975bbfbf18f6447a599550edb052e52264fb7124d04a12e6175e330a5.da.png)

### Trin 2: Opret din `.env`-fil

For at oprette din `.env`-fil skal du køre følgende kommando i din terminal.

```bash
cp .env.example .env
```

Dette vil kopiere eksempel-filen og oprette en `.env` i din mappe, hvor du kan udfylde værdierne for miljøvariablerne.

Med din token kopieret, skal du åbne `.env`-filen i din foretrukne teksteditor og indsætte din token i `PROJECT_ENDPOINT`-feltet.

### Trin 3: Log ind på Azure

Som en sikkerhedsforanstaltning vil vi bruge [keyless authentication](https://learn.microsoft.com/azure/developer/ai/keyless-connections?tabs=csharp%2Cazure-cli?WT.mc_id=academic-105485-koreyst) til at autentificere til Azure OpenAI med Microsoft Entra ID.

Åbn derefter en terminal og kør `az login --use-device-code` for at logge ind på din Azure-konto.

Når du er logget ind, skal du vælge dit abonnement i terminalen.

## Yderligere miljøvariabler - Azure Search og Azure OpenAI

Til Agentic RAG-lektionen - Lektion 5 - er der eksempler, der bruger Azure Search og Azure OpenAI.

Hvis du vil køre disse eksempler, skal du tilføje følgende miljøvariabler til din `.env`-fil:

### Oversigtsside (Projekt)

- `AZURE_SUBSCRIPTION_ID` - Tjek **Project details** på **Overview**-siden for dit projekt.

- `AZURE_AI_PROJECT_NAME` - Se øverst på **Overview**-siden for dit projekt.

- `AZURE_OPENAI_SERVICE` - Find dette under **Included capabilities**-fanen for **Azure OpenAI Service** på **Overview**-siden.

### Management Center

- `AZURE_OPENAI_RESOURCE_GROUP` - Gå til **Project properties** på **Overview**-siden for **Management Center**.

- `GLOBAL_LLM_SERVICE` - Under **Connected resources**, find navnet på **Azure AI Services**-forbindelsen. Hvis det ikke er angivet, skal du tjekke **Azure portal** under din ressourcegruppe for navnet på AI Services-ressourcen.

### Models + Endpoints-side

- `AZURE_OPENAI_EMBEDDING_DEPLOYMENT_NAME` - Vælg din embedding-model (f.eks. `text-embedding-ada-002`) og noter **Deployment name** fra modeldetaljerne.

- `AZURE_OPENAI_CHAT_DEPLOYMENT_NAME` - Vælg din chat-model (f.eks. `gpt-4o-mini`) og noter **Deployment name** fra modeldetaljerne.

### Azure Portal

- `AZURE_OPENAI_ENDPOINT` - Find **Azure AI services**, klik på det, gå derefter til **Resource Management**, **Keys and Endpoint**, scroll ned til "Azure OpenAI endpoints", og kopier den, der siger "Language APIs".

- `AZURE_OPENAI_API_KEY` - Fra samme skærm, kopier KEY 1 eller KEY 2.

- `AZURE_SEARCH_SERVICE_ENDPOINT` - Find din **Azure AI Search**-ressource, klik på den, og se **Overview**.

- `AZURE_SEARCH_API_KEY` - Gå derefter til **Settings** og derefter **Keys** for at kopiere den primære eller sekundære admin-nøgle.

### Ekstern webside

- `AZURE_OPENAI_API_VERSION` - Besøg siden [API version lifecycle](https://learn.microsoft.com/en-us/azure/ai-services/openai/api-version-deprecation#latest-ga-api-release) under **Latest GA API release**.

### Opsætning af keyless authentication

I stedet for at hardkode dine legitimationsoplysninger, vil vi bruge en keyless-forbindelse med Azure OpenAI. For at gøre dette vil vi importere `DefaultAzureCredential` og senere kalde funktionen `DefaultAzureCredential` for at få legitimationsoplysningerne.

```python
from azure.identity import DefaultAzureCredential, InteractiveBrowserCredential
```

## Sidder du fast?

Hvis du har problemer med at køre denne opsætning, så hop ind i vores

## Næste lektion

Du er nu klar til at køre koden for dette kursus. God fornøjelse med at lære mere om AI-agenter!  

[Introduktion til AI-agenter og agentanvendelser](../01-intro-to-ai-agents/README.md)

---

**Ansvarsfraskrivelse**:  
Dette dokument er blevet oversat ved hjælp af AI-oversættelsestjenesten [Co-op Translator](https://github.com/Azure/co-op-translator). Selvom vi bestræber os på nøjagtighed, skal du være opmærksom på, at automatiserede oversættelser kan indeholde fejl eller unøjagtigheder. Det originale dokument på dets oprindelige sprog bør betragtes som den autoritative kilde. For kritisk information anbefales professionel menneskelig oversættelse. Vi påtager os intet ansvar for misforståelser eller fejltolkninger, der måtte opstå som følge af brugen af denne oversættelse.