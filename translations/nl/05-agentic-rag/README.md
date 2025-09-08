<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "d2f04b783b9e1253100329afd698f8ff",
  "translation_date": "2025-08-29T17:27:41+00:00",
  "source_file": "05-agentic-rag/README.md",
  "language_code": "nl"
}
-->
[![Agentic RAG](../../../translated_images/lesson-5-thumbnail.20ba9d0c0ae64fae06637eb2023395d437b0152c0463c2227ff456afe5f14644.nl.png)](https://youtu.be/WcjAARvdL7I?si=BCgwjwFb2yCkEhR9)

> _(Klik op de afbeelding hierboven om de video van deze les te bekijken)_

# Agentic RAG

Deze les biedt een uitgebreide introductie tot Agentic Retrieval-Augmented Generation (Agentic RAG), een opkomend AI-paradigma waarbij grote taalmodellen (LLMs) autonoom hun volgende stappen plannen terwijl ze informatie ophalen uit externe bronnen. In tegenstelling tot statische patronen van ophalen en lezen, omvat Agentic RAG iteratieve oproepen naar het LLM, afgewisseld met tool- of functieoproepen en gestructureerde outputs. Het systeem evalueert resultaten, verfijnt zoekopdrachten, roept indien nodig extra tools aan en herhaalt deze cyclus totdat een bevredigende oplossing is bereikt.

## Introductie

Deze les behandelt:

- **Begrijp Agentic RAG:** Leer over het opkomende paradigma in AI waarbij grote taalmodellen (LLMs) autonoom hun volgende stappen plannen terwijl ze informatie ophalen uit externe databronnen.
- **Begrijp Iteratieve Maker-Checker Stijl:** Begrijp de iteratieve cyclus van oproepen naar het LLM, afgewisseld met tool- of functieoproepen en gestructureerde outputs, ontworpen om de nauwkeurigheid te verbeteren en foutieve zoekopdrachten te corrigeren.
- **Verken Praktische Toepassingen:** Identificeer scenario's waarin Agentic RAG uitblinkt, zoals omgevingen waar nauwkeurigheid voorop staat, complexe database-interacties en uitgebreide workflows.

## Leerdoelen

Na het voltooien van deze les weet je hoe je:

- **Agentic RAG begrijpt:** Leer over het opkomende paradigma in AI waarbij grote taalmodellen (LLMs) autonoom hun volgende stappen plannen terwijl ze informatie ophalen uit externe databronnen.
- **Iteratieve Maker-Checker Stijl:** Begrijp het concept van een iteratieve cyclus van oproepen naar het LLM, afgewisseld met tool- of functieoproepen en gestructureerde outputs, ontworpen om de nauwkeurigheid te verbeteren en foutieve zoekopdrachten te corrigeren.
- **Het redeneerproces beheren:** Begrijp het vermogen van het systeem om zijn eigen redeneerproces te beheren, beslissingen te nemen over hoe problemen aan te pakken zonder te vertrouwen op vooraf gedefinieerde paden.
- **Workflow:** Begrijp hoe een agentisch model zelfstandig besluit om markttrendrapporten op te halen, concurrentiedata te identificeren, interne verkoopstatistieken te correleren, bevindingen te synthetiseren en de strategie te evalueren.
- **Iteratieve loops, toolintegratie en geheugen:** Leer over de afhankelijkheid van het systeem van een interactiepatroon met loops, waarbij het status en geheugen behoudt over stappen om herhaling te vermijden en geïnformeerde beslissingen te nemen.
- **Omgaan met faalmodi en zelfcorrectie:** Verken de robuuste zelfcorrectiemechanismen van het systeem, waaronder itereren en opnieuw zoeken, diagnostische tools gebruiken en terugvallen op menselijke controle.
- **Grenzen van autonomie:** Begrijp de beperkingen van Agentic RAG, met de nadruk op domeinspecifieke autonomie, afhankelijkheid van infrastructuur en respect voor veiligheidsmaatregelen.
- **Praktische toepassingen en waarde:** Identificeer scenario's waarin Agentic RAG uitblinkt, zoals omgevingen waar nauwkeurigheid voorop staat, complexe database-interacties en uitgebreide workflows.
- **Governance, transparantie en vertrouwen:** Leer over het belang van governance en transparantie, inclusief uitlegbaar redeneren, biascontrole en menselijke controle.

## Wat is Agentic RAG?

Agentic Retrieval-Augmented Generation (Agentic RAG) is een opkomend AI-paradigma waarbij grote taalmodellen (LLMs) autonoom hun volgende stappen plannen terwijl ze informatie ophalen uit externe bronnen. In tegenstelling tot statische patronen van ophalen en lezen, omvat Agentic RAG iteratieve oproepen naar het LLM, afgewisseld met tool- of functieoproepen en gestructureerde outputs. Het systeem evalueert resultaten, verfijnt zoekopdrachten, roept indien nodig extra tools aan en herhaalt deze cyclus totdat een bevredigende oplossing is bereikt. Deze iteratieve “maker-checker” stijl verbetert de nauwkeurigheid, corrigeert foutieve zoekopdrachten en zorgt voor hoogwaardige resultaten.

Het systeem beheert actief zijn redeneerproces, herschrijft mislukte zoekopdrachten, kiest verschillende ophaalmethoden en integreert meerdere tools—zoals vectorzoekopdrachten in Azure AI Search, SQL-databases of aangepaste API's—voordat het zijn antwoord afrondt. De onderscheidende eigenschap van een agentisch systeem is het vermogen om zijn eigen redeneerproces te beheren. Traditionele RAG-implementaties vertrouwen op vooraf gedefinieerde paden, maar een agentisch systeem bepaalt autonoom de volgorde van stappen op basis van de kwaliteit van de gevonden informatie.

## Definitie van Agentic Retrieval-Augmented Generation (Agentic RAG)

Agentic Retrieval-Augmented Generation (Agentic RAG) is een opkomend paradigma in AI-ontwikkeling waarbij LLMs niet alleen informatie ophalen uit externe databronnen, maar ook autonoom hun volgende stappen plannen. In tegenstelling tot statische patronen van ophalen en lezen of zorgvuldig gescripte promptreeksen, omvat Agentic RAG een cyclus van iteratieve oproepen naar het LLM, afgewisseld met tool- of functieoproepen en gestructureerde outputs. Bij elke stap evalueert het systeem de verkregen resultaten, beslist of het zoekopdrachten moet verfijnen, roept indien nodig extra tools aan en herhaalt deze cyclus totdat een bevredigende oplossing is bereikt.

Deze iteratieve “maker-checker” stijl van werken is ontworpen om de nauwkeurigheid te verbeteren, foutieve zoekopdrachten naar gestructureerde databases (bijv. NL2SQL) te corrigeren en gebalanceerde, hoogwaardige resultaten te garanderen. In plaats van uitsluitend te vertrouwen op zorgvuldig ontworpen promptketens, beheert het systeem actief zijn redeneerproces. Het kan zoekopdrachten herschrijven die mislukken, verschillende ophaalmethoden kiezen en meerdere tools integreren—zoals vectorzoekopdrachten in Azure AI Search, SQL-databases of aangepaste API's—voordat het zijn antwoord afrondt. Dit elimineert de noodzaak voor overdreven complexe orkestratiekaders. In plaats daarvan kan een relatief eenvoudige cyclus van “LLM-oproep → toolgebruik → LLM-oproep → …” leiden tot verfijnde en goed onderbouwde outputs.

![Agentic RAG Core Loop](../../../translated_images/agentic-rag-core-loop.c8f4b85c26920f71ed181ebb14001ac7aae47c0b0af237edcf71898645a62db3.nl.png)

## Het redeneerproces beheren

De onderscheidende eigenschap die een systeem “agentisch” maakt, is het vermogen om zijn redeneerproces te beheren. Traditionele RAG-implementaties vertrouwen vaak op mensen om een pad voor het model vooraf te definiëren: een chain-of-thought die aangeeft wat te halen en wanneer. Maar wanneer een systeem echt agentisch is, beslist het intern hoe het probleem moet worden aangepakt. Het voert niet alleen een script uit; het bepaalt autonoom de volgorde van stappen op basis van de kwaliteit van de gevonden informatie.

Bijvoorbeeld, als het wordt gevraagd om een strategie voor een productlancering te creëren, vertrouwt het niet alleen op een prompt die de hele onderzoeks- en besluitvormingsworkflow beschrijft. In plaats daarvan besluit het agentische model zelfstandig om:

1. Actuele markttrendrapporten op te halen via Bing Web Grounding.
2. Relevante concurrentiedata te identificeren via Azure AI Search.
3. Historische interne verkoopstatistieken te correleren via Azure SQL Database.
4. De bevindingen te synthetiseren tot een samenhangende strategie, georkestreerd via Azure OpenAI Service.
5. De strategie te evalueren op hiaten of inconsistenties, wat kan leiden tot een nieuwe ronde van ophalen indien nodig.

Al deze stappen—zoekopdrachten verfijnen, bronnen kiezen, itereren totdat het “tevreden” is met het antwoord—worden door het model zelf beslist, niet vooraf gescript door een mens.

## Iteratieve loops, toolintegratie en geheugen

![Tool Integration Architecture](../../../translated_images/tool-integration.0f569710b5c17c106757adba082f6c4be025ca0721bff7d1ee4b929a3617a600.nl.png)

Een agentisch systeem vertrouwt op een interactiepatroon met loops:

- **Initiële oproep:** Het doel van de gebruiker (ook wel gebruikersprompt genoemd) wordt aan het LLM gepresenteerd.
- **Toolgebruik:** Als het model ontbrekende informatie of onduidelijke instructies identificeert, selecteert het een tool of ophaalmethode—zoals een vectorzoekopdracht (bijv. Azure AI Search Hybrid search over privédata) of een gestructureerde SQL-oproep—om meer context te verzamelen.
- **Beoordeling & verfijning:** Na het beoordelen van de teruggestuurde data beslist het model of de informatie voldoende is. Zo niet, dan verfijnt het de zoekopdracht, probeert een andere tool of past zijn aanpak aan.
- **Herhaal tot tevreden:** Deze cyclus gaat door totdat het model bepaalt dat het voldoende duidelijkheid en bewijs heeft om een definitief, goed onderbouwd antwoord te geven.
- **Geheugen & status:** Omdat het systeem status en geheugen behoudt over stappen, kan het eerdere pogingen en hun resultaten herinneren, herhaling vermijden en meer geïnformeerde beslissingen nemen naarmate het verder gaat.

Na verloop van tijd creëert dit een gevoel van evoluerend begrip, waardoor het model complexe, meerstaps taken kan navigeren zonder dat een mens constant hoeft in te grijpen of de prompt opnieuw moet vormgeven.

## Omgaan met faalmodi en zelfcorrectie

De autonomie van Agentic RAG omvat ook robuuste zelfcorrectiemechanismen. Wanneer het systeem op doodlopende wegen stuit—zoals het ophalen van irrelevante documenten of het tegenkomen van foutieve zoekopdrachten—kan het:

- **Itereren en opnieuw zoeken:** In plaats van antwoorden van lage waarde te retourneren, probeert het model nieuwe zoekstrategieën, herschrijft databasezoekopdrachten of bekijkt alternatieve datasets.
- **Diagnostische tools gebruiken:** Het systeem kan extra functies oproepen die zijn ontworpen om het te helpen zijn redeneerprocessen te debuggen of de juistheid van opgehaalde data te bevestigen. Tools zoals Azure AI Tracing zullen belangrijk zijn om robuuste observatie en monitoring mogelijk te maken.
- **Terugvallen op menselijke controle:** Voor scenario's met hoge inzet of herhaaldelijk falen kan het model onzekerheid aangeven en om menselijke begeleiding vragen. Zodra de mens corrigerende feedback geeft, kan het model die les voortaan meenemen.

Deze iteratieve en dynamische aanpak stelt het model in staat om continu te verbeteren, waardoor het niet slechts een eenmalig systeem is, maar een systeem dat leert van zijn misstappen tijdens een sessie.

![Self Correction Mechanism](../../../translated_images/self-correction.da87f3783b7f174bdc592c754b352884dd283814758bfeb7a68f5fd910272f3b.nl.png)

## Grenzen van autonomie

Ondanks zijn autonomie binnen een taak, is Agentic RAG niet vergelijkbaar met Kunstmatige Algemene Intelligentie. Zijn “agentische” capaciteiten zijn beperkt tot de tools, databronnen en beleidsregels die door menselijke ontwikkelaars worden geleverd. Het kan geen eigen tools uitvinden of buiten de domeingrenzen treden die zijn ingesteld. In plaats daarvan blinkt het uit in het dynamisch orkestreren van de beschikbare middelen.

Belangrijke verschillen met meer geavanceerde AI-vormen zijn:

1. **Domeinspecifieke autonomie:** Agentic RAG-systemen zijn gericht op het bereiken van door de gebruiker gedefinieerde doelen binnen een bekend domein, waarbij strategieën zoals zoekopdrachten herschrijven of toolselectie worden gebruikt om de resultaten te verbeteren.
2. **Afhankelijk van infrastructuur:** De capaciteiten van het systeem hangen af van de tools en data die door ontwikkelaars zijn geïntegreerd. Het kan deze grenzen niet overschrijden zonder menselijke tussenkomst.
3. **Respect voor veiligheidsmaatregelen:** Ethische richtlijnen, nalevingsregels en bedrijfsbeleid blijven erg belangrijk. De vrijheid van de agent is altijd beperkt door veiligheidsmaatregelen en controlemechanismen (hopelijk?).

## Praktische toepassingen en waarde

Agentic RAG blinkt uit in scenario's die iteratieve verfijning en precisie vereisen:

1. **Omgevingen waar nauwkeurigheid voorop staat:** Bij nalevingscontroles, regelgevingsanalyses of juridisch onderzoek kan het agentische model feiten herhaaldelijk verifiëren, meerdere bronnen raadplegen en zoekopdrachten herschrijven totdat het een grondig gecontroleerd antwoord produceert.
2. **Complexe database-interacties:** Bij gestructureerde data waar zoekopdrachten vaak kunnen mislukken of moeten worden aangepast, kan het systeem zelfstandig zijn zoekopdrachten verfijnen met Azure SQL of Microsoft Fabric OneLake, zodat de uiteindelijke resultaten aansluiten bij de intentie van de gebruiker.
3. **Uitgebreide workflows:** Langdurige sessies kunnen evolueren naarmate nieuwe informatie beschikbaar komt. Agentic RAG kan continu nieuwe data integreren en strategieën aanpassen naarmate het meer leert over het probleemgebied.

## Governance, transparantie en vertrouwen

Naarmate deze systemen autonomer worden in hun redeneerprocessen, zijn governance en transparantie cruciaal:

- **Uitlegbaar redeneren:** Het model kan een audittrail bieden van de zoekopdrachten die het heeft uitgevoerd, de bronnen die het heeft geraadpleegd en de redeneerprocessen die het heeft gevolgd om tot zijn conclusie te komen. Tools zoals Azure AI Content Safety en Azure AI Tracing / GenAIOps kunnen helpen transparantie te behouden en risico's te beperken.
- **Biascontrole en gebalanceerd ophalen:** Ontwikkelaars kunnen ophaalstrategieën afstemmen om ervoor te zorgen dat gebalanceerde, representatieve databronnen worden overwogen, en outputs regelmatig auditen om bias of scheve patronen te detecteren met behulp van aangepaste modellen voor geavanceerde data science-organisaties die Azure Machine Learning gebruiken.
- **Menselijke controle en naleving:** Voor gevoelige taken blijft menselijke beoordeling essentieel. Agentic RAG vervangt geen menselijke oordeelsvorming bij beslissingen met hoge inzet—het versterkt deze door meer grondig gecontroleerde opties te leveren.

Het hebben van tools die een duidelijk overzicht van acties bieden is essentieel. Zonder deze tools kan het debuggen van een meerstapsproces erg moeilijk zijn. Zie het volgende voorbeeld van Literal AI (bedrijf achter Chainlit) voor een Agent-run:

![AgentRunExample](../../../translated_images/AgentRunExample.471a94bc40cbdc0cd04c1f43c8d8c9b751f10d97918c900e29cb3ba0d6aa4c00.nl.png)

![AgentRunExample2](../../../translated_images/AgentRunExample2.19c7410a03bbc216c446b8a4e35ac82f1e8bc0ed313484212f5f4d1137637245.nl.png)

## Conclusie

Agentic RAG vertegenwoordigt een natuurlijke evolutie in hoe AI-systemen complexe, data-intensieve taken aanpakken. Door een interactiepatroon met loops te adopteren, autonoom tools te selecteren en zoekopdrachten te verfijnen totdat een hoogwaardig resultaat is bereikt, gaat het systeem verder dan statisch prompt-volgen naar een meer adaptieve, contextbewuste besluitvormer. Hoewel het nog steeds beperkt is door menselijk gedefinieerde infrastructuren en ethische richtlijnen, maken deze agentische capaciteiten rijkere, dynamischere en uiteindelijk nuttigere AI-interacties mogelijk voor zowel bedrijven als eindgebruikers.

### Meer vragen over Agentic RAG?

Word lid van de [Azure AI Foundry Discord](https://aka.ms/ai-agents/discord) om andere leerlingen te ontmoeten, kantooruren bij te wonen en je vragen over AI Agents beantwoord te krijgen.

## Aanvullende bronnen

-
<a href="https://learn.microsoft.com/training/modules/use-own-data-azure-openai" target="_blank">
Implementeer Retrieval Augmented Generation (RAG) met Azure OpenAI Service: Leer hoe je je eigen data kunt gebruiken met de Azure OpenAI Service. Deze Microsoft Learn-module biedt een uitgebreide gids voor het implementeren van RAG  
- <a href="https://learn.microsoft.com/azure/ai-studio/concepts/evaluation-approach-gen-ai" target="_blank">Evaluatie van generatieve AI-toepassingen met Azure AI Foundry: Dit artikel behandelt de evaluatie en vergelijking van modellen op openbaar beschikbare datasets, inclusief Agentic AI-toepassingen en RAG-architecturen</a>  
- <a href="https://weaviate.io/blog/what-is-agentic-rag" target="_blank">Wat is Agentic RAG | Weaviate</a>  
- <a href="https://ragaboutit.com/agentic-rag-a-complete-guide-to-agent-based-retrieval-augmented-generation/" target="_blank">Agentic RAG: Een complete gids voor agent-gebaseerde Retrieval Augmented Generation – Nieuws over generatie RAG</a>  
- <a href="https://huggingface.co/learn/cookbook/agent_rag" target="_blank">Agentic RAG: geef je RAG een boost met query-herformulering en zelf-query! Hugging Face Open-Source AI Cookbook</a>  
- <a href="https://youtu.be/aQ4yQXeB1Ss?si=2HUqBzHoeB5tR04U" target="_blank">Agentic lagen toevoegen aan RAG</a>  
- <a href="https://www.youtube.com/watch?v=zeAyuLc_f3Q&t=244s" target="_blank">De toekomst van kennisassistenten: Jerry Liu</a>  
- <a href="https://www.youtube.com/watch?v=AOSjiXP1jmQ" target="_blank">Hoe bouw je Agentic RAG-systemen</a>  
- <a href="https://ignite.microsoft.com/sessions/BRK102?source=sessions" target="_blank">Azure AI Foundry Agent Service gebruiken om je AI-agents op te schalen</a>  

### Academische Artikelen  

- <a href="https://arxiv.org/abs/2303.17651" target="_blank">2303.17651 Self-Refine: Iteratieve verfijning met zelf-feedback</a>  
- <a href="https://arxiv.org/abs/2303.11366" target="_blank">2303.11366 Reflexion: Taalagents met verbale versterkingsleren</a>  
- <a href="https://arxiv.org/abs/2305.11738" target="_blank">2305.11738 CRITIC: Grote taalmodellen kunnen zichzelf corrigeren met tool-interactieve kritiek</a>  
- <a href="https://arxiv.org/abs/2501.09136" target="_blank">2501.09136 Agentic Retrieval-Augmented Generation: Een overzicht van Agentic RAG</a>  

## Vorige Les  

[Tool Use Design Pattern](../04-tool-use/README.md)  

## Volgende Les  

[Vertrouwenswaardige AI-agents bouwen](../06-building-trustworthy-agents/README.md)  

---

**Disclaimer**:  
Dit document is vertaald met behulp van de AI-vertalingsservice [Co-op Translator](https://github.com/Azure/co-op-translator). Hoewel we ons best doen voor nauwkeurigheid, dient u zich ervan bewust te zijn dat geautomatiseerde vertalingen fouten of onnauwkeurigheden kunnen bevatten. Het originele document in zijn oorspronkelijke taal moet worden beschouwd als de gezaghebbende bron. Voor cruciale informatie wordt professionele menselijke vertaling aanbevolen. Wij zijn niet aansprakelijk voor misverstanden of verkeerde interpretaties die voortvloeien uit het gebruik van deze vertaling.