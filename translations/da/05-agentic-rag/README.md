<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "d2f04b783b9e1253100329afd698f8ff",
  "translation_date": "2025-08-29T15:41:59+00:00",
  "source_file": "05-agentic-rag/README.md",
  "language_code": "da"
}
-->
[![Agentic RAG](../../../translated_images/lesson-5-thumbnail.20ba9d0c0ae64fae06637eb2023395d437b0152c0463c2227ff456afe5f14644.da.png)](https://youtu.be/WcjAARvdL7I?si=BCgwjwFb2yCkEhR9)

> _(Klik på billedet ovenfor for at se videoen til denne lektion)_

# Agentic RAG

Denne lektion giver en omfattende introduktion til Agentic Retrieval-Augmented Generation (Agentic RAG), et nyt AI-paradigme, hvor store sprogmodeller (LLMs) selvstændigt planlægger deres næste skridt, mens de henter information fra eksterne kilder. I modsætning til statiske retrieval-then-read-mønstre involverer Agentic RAG iterative opkald til LLM'en, afbrudt af værktøjs- eller funktionskald og strukturerede outputs. Systemet evaluerer resultater, forfiner forespørgsler, anvender yderligere værktøjer, hvis nødvendigt, og fortsætter denne cyklus, indtil en tilfredsstillende løsning er opnået.

## Introduktion

Denne lektion vil dække:

- **Forstå Agentic RAG:** Lær om det nye paradigme inden for AI, hvor store sprogmodeller (LLMs) selvstændigt planlægger deres næste skridt, mens de henter information fra eksterne datakilder.
- **Forstå Iterativ Maker-Checker Stil:** Forstå loopet af iterative opkald til LLM'en, afbrudt af værktøjs- eller funktionskald og strukturerede outputs, designet til at forbedre korrekthed og håndtere fejlbehæftede forespørgsler.
- **Udforsk Praktiske Anvendelser:** Identificer scenarier, hvor Agentic RAG udmærker sig, såsom korrekthedsorienterede miljøer, komplekse databaseinteraktioner og udvidede arbejdsgange.

## Læringsmål

Efter at have gennemført denne lektion vil du vide, hvordan du/forstå:

- **Forståelse af Agentic RAG:** Lær om det nye paradigme inden for AI, hvor store sprogmodeller (LLMs) selvstændigt planlægger deres næste skridt, mens de henter information fra eksterne datakilder.
- **Iterativ Maker-Checker Stil:** Forstå konceptet med et loop af iterative opkald til LLM'en, afbrudt af værktøjs- eller funktionskald og strukturerede outputs, designet til at forbedre korrekthed og håndtere fejlbehæftede forespørgsler.
- **Eje Beslutningsprocessen:** Forstå systemets evne til at eje sin beslutningsproces og træffe beslutninger om, hvordan problemer skal tackles uden at være afhængig af foruddefinerede veje.
- **Arbejdsgang:** Forstå, hvordan en agentisk model selvstændigt beslutter at hente markedsrapporter, identificere konkurrentdata, korrelere interne salgsdata, syntetisere resultater og evaluere strategien.
- **Iterative Loops, Værktøjsintegration og Hukommelse:** Lær om systemets afhængighed af et loop-interaktionsmønster, der opretholder tilstand og hukommelse på tværs af trin for at undgå gentagelser og træffe informerede beslutninger.
- **Håndtering af Fejltilstande og Selvkorrektion:** Udforsk systemets robuste selvkorrigeringsmekanismer, herunder iteration og genforespørgsel, brug af diagnostiske værktøjer og tilbagefald til menneskelig overvågning.
- **Grænser for Agentic RAG:** Forstå begrænsningerne ved Agentic RAG med fokus på domænespecifik autonomi, afhængighed af infrastruktur og respekt for sikkerhedsforanstaltninger.
- **Praktiske Anvendelser og Værdi:** Identificer scenarier, hvor Agentic RAG udmærker sig, såsom korrekthedsorienterede miljøer, komplekse databaseinteraktioner og udvidede arbejdsgange.
- **Styring, Gennemsigtighed og Tillid:** Lær om vigtigheden af styring og gennemsigtighed, herunder forklarlig beslutningstagning, kontrol af bias og menneskelig overvågning.

## Hvad er Agentic RAG?

Agentic Retrieval-Augmented Generation (Agentic RAG) er et nyt AI-paradigme, hvor store sprogmodeller (LLMs) selvstændigt planlægger deres næste skridt, mens de henter information fra eksterne kilder. I modsætning til statiske retrieval-then-read-mønstre involverer Agentic RAG iterative opkald til LLM'en, afbrudt af værktøjs- eller funktionskald og strukturerede outputs. Systemet evaluerer resultater, forfiner forespørgsler, anvender yderligere værktøjer, hvis nødvendigt, og fortsætter denne cyklus, indtil en tilfredsstillende løsning er opnået. Denne iterative “maker-checker”-stil forbedrer korrekthed, håndterer fejlbehæftede forespørgsler og sikrer resultater af høj kvalitet.

Systemet tager aktivt ejerskab over sin beslutningsproces, omskriver fejlede forespørgsler, vælger forskellige metoder til informationshentning og integrerer flere værktøjer—såsom vektorsøgning i Azure AI Search, SQL-databaser eller brugerdefinerede API'er—før det færdiggør sit svar. Den afgørende kvalitet ved et agentisk system er dets evne til at eje sin beslutningsproces. Traditionelle RAG-implementeringer er afhængige af foruddefinerede veje, men et agentisk system bestemmer selv rækkefølgen af trin baseret på kvaliteten af den information, det finder.

## Definition af Agentic Retrieval-Augmented Generation (Agentic RAG)

Agentic Retrieval-Augmented Generation (Agentic RAG) er et nyt paradigme inden for AI-udvikling, hvor LLM'er ikke kun henter information fra eksterne datakilder, men også selvstændigt planlægger deres næste skridt. I modsætning til statiske retrieval-then-read-mønstre eller nøje scriptede promptsekvenser involverer Agentic RAG et loop af iterative opkald til LLM'en, afbrudt af værktøjs- eller funktionskald og strukturerede outputs. Ved hver iteration evaluerer systemet de opnåede resultater, beslutter, om forespørgsler skal forfines, anvender yderligere værktøjer, hvis nødvendigt, og fortsætter denne cyklus, indtil en tilfredsstillende løsning er opnået.

Denne iterative “maker-checker”-stil er designet til at forbedre korrekthed, håndtere fejlbehæftede forespørgsler til strukturerede databaser (f.eks. NL2SQL) og sikre balancerede, høj-kvalitets resultater. I stedet for kun at stole på nøje udformede promptkæder tager systemet aktivt ejerskab over sin beslutningsproces. Det kan omskrive fejlede forespørgsler, vælge forskellige metoder til informationshentning og integrere flere værktøjer—såsom vektorsøgning i Azure AI Search, SQL-databaser eller brugerdefinerede API'er—før det færdiggør sit svar. Dette eliminerer behovet for overdrevent komplekse orkestreringsrammer. I stedet kan en relativt simpel loop af “LLM-opkald → værktøjsbrug → LLM-opkald → …” resultere i sofistikerede og velbegrundede outputs.

![Agentic RAG Core Loop](../../../translated_images/agentic-rag-core-loop.c8f4b85c26920f71ed181ebb14001ac7aae47c0b0af237edcf71898645a62db3.da.png)

## Ejerskab af Beslutningsprocessen

Den afgørende kvalitet, der gør et system “agentisk,” er dets evne til at eje sin beslutningsproces. Traditionelle RAG-implementeringer er ofte afhængige af, at mennesker foruddefinerer en sti for modellen: en ræsonnementskæde, der beskriver, hvad der skal hentes, og hvornår.
Men når et system er virkelig agentisk, beslutter det internt, hvordan det skal gribe problemet an. Det udfører ikke bare et script; det bestemmer selv rækkefølgen af trin baseret på kvaliteten af den information, det finder.
For eksempel, hvis det bliver bedt om at udarbejde en produktlanceringsstrategi, er det ikke kun afhængigt af en prompt, der beskriver hele forsknings- og beslutningsarbejdsgangen. I stedet beslutter den agentiske model selvstændigt at:

1. Hente aktuelle markedsrapporter ved hjælp af Bing Web Grounding.
2. Identificere relevante konkurrentdata ved hjælp af Azure AI Search.
3. Korrelere historiske interne salgsdata ved hjælp af Azure SQL Database.
4. Syntetisere resultaterne til en sammenhængende strategi orkestreret via Azure OpenAI Service.
5. Evaluere strategien for mangler eller inkonsistenser og igangsætte en ny runde af informationshentning, hvis nødvendigt.
Alle disse trin—at forfine forespørgsler, vælge kilder, iterere, indtil svaret er tilfredsstillende—besluttes af modellen og er ikke foruddefineret af et menneske.

## Iterative Loops, Værktøjsintegration og Hukommelse

![Tool Integration Architecture](../../../translated_images/tool-integration.0f569710b5c17c106757adba082f6c4be025ca0721bff7d1ee4b929a3617a600.da.png)

Et agentisk system er afhængigt af et loop-interaktionsmønster:

- **Første Opkald:** Brugerens mål (dvs. brugerens prompt) præsenteres for LLM'en.
- **Værktøjsanvendelse:** Hvis modellen identificerer manglende information eller uklare instruktioner, vælger den et værktøj eller en metode til informationshentning—som en vektordatabaseforespørgsel (f.eks. Azure AI Search Hybrid-søgning over private data) eller et struktureret SQL-opkald—for at indsamle mere kontekst.
- **Vurdering og Forfining:** Efter at have gennemgået de returnerede data beslutter modellen, om informationen er tilstrækkelig. Hvis ikke, forfiner den forespørgslen, prøver et andet værktøj eller justerer sin tilgang.
- **Gentag Indtil Tilfreds:** Denne cyklus fortsætter, indtil modellen vurderer, at den har tilstrækkelig klarhed og evidens til at levere et endeligt, velbegrundet svar.
- **Hukommelse og Tilstand:** Fordi systemet opretholder tilstand og hukommelse på tværs af trin, kan det huske tidligere forsøg og deres resultater, undgå gentagelser og træffe mere informerede beslutninger, efterhånden som det skrider frem.

Over tid skaber dette en følelse af udviklende forståelse, der gør det muligt for modellen at navigere komplekse, flertrinsopgaver uden konstant menneskelig indgriben eller omformulering af prompten.

## Håndtering af Fejltilstande og Selvkorrektion

Agentic RAG’s autonomi indebærer også robuste selvkorrigeringsmekanismer. Når systemet støder på blindgyder—såsom at hente irrelevante dokumenter eller støde på fejlbehæftede forespørgsler—kan det:

- **Iterere og Genforespørge:** I stedet for at returnere lavværdi-svar forsøger modellen nye søgestrategier, omskriver databaseforespørgsler eller undersøger alternative datasæt.
- **Brug Diagnostiske Værktøjer:** Systemet kan anvende yderligere funktioner designet til at hjælpe det med at fejlfinde sine ræsonnementstrin eller bekræfte korrektheden af hentede data. Værktøjer som Azure AI Tracing vil være vigtige for at muliggøre robust overvågning og sporing.
- **Tilbagefald til Menneskelig Overvågning:** For opgaver med høj risiko eller gentagne fejl kan modellen markere usikkerhed og anmode om menneskelig vejledning. Når mennesket giver korrigerende feedback, kan modellen inkorporere denne læring fremadrettet.

Denne iterative og dynamiske tilgang gør det muligt for modellen at forbedre sig kontinuerligt og sikrer, at den ikke bare er et engangssystem, men et system, der lærer af sine fejltrin under en given session.

![Self Correction Mechanism](../../../translated_images/self-correction.da87f3783b7f174bdc592c754b352884dd283814758bfeb7a68f5fd910272f3b.da.png)

## Grænser for Agentic RAG

På trods af sin autonomi inden for en opgave er Agentic RAG ikke det samme som Artificial General Intelligence. Dens “agentiske” evner er begrænset til de værktøjer, datakilder og politikker, som menneskelige udviklere stiller til rådighed. Den kan ikke opfinde sine egne værktøjer eller træde uden for de domænegrænser, der er fastsat. I stedet udmærker den sig ved dynamisk at orkestrere de ressourcer, den har til rådighed.
Vigtige forskelle fra mere avancerede AI-former inkluderer:

1. **Domænespecifik Autonomi:** Agentic RAG-systemer fokuserer på at opnå brugerdefinerede mål inden for et kendt domæne og anvender strategier som omskrivning af forespørgsler eller værktøjsvalg for at forbedre resultater.
2. **Afhængighed af Infrastruktur:** Systemets evner afhænger af de værktøjer og data, som udviklere integrerer. Det kan ikke overskride disse grænser uden menneskelig indgriben.
3. **Respekt for Sikkerhedsforanstaltninger:** Etiske retningslinjer, overholdelsesregler og forretningspolitikker forbliver meget vigtige. Agentens frihed er altid begrænset af sikkerhedsforanstaltninger og overvågningsmekanismer (forhåbentlig?).

## Praktiske Anvendelser og Værdi

Agentic RAG udmærker sig i scenarier, der kræver iterativ forfining og præcision:

1. **Korrekthedsorienterede Miljøer:** I overholdelseskontrol, regulatorisk analyse eller juridisk forskning kan den agentiske model gentagne gange verificere fakta, konsultere flere kilder og omskrive forespørgsler, indtil den producerer et grundigt gennemgået svar.
2. **Komplekse Databaseinteraktioner:** Når der arbejdes med strukturerede data, hvor forespørgsler ofte kan fejle eller kræve justering, kan systemet selvstændigt forfine sine forespørgsler ved hjælp af Azure SQL eller Microsoft Fabric OneLake og sikre, at den endelige hentning stemmer overens med brugerens hensigt.
3. **Udvidede Arbejdsgange:** Længerevarende sessioner kan udvikle sig, efterhånden som ny information dukker op. Agentic RAG kan løbende inkorporere nye data og ændre strategier, efterhånden som den lærer mere om problemområdet.

## Styring, Gennemsigtighed og Tillid

Efterhånden som disse systemer bliver mere selvstændige i deres ræsonnement, er styring og gennemsigtighed afgørende:

- **Forklarlig Ræsonnering:** Modellen kan give en revisionsspor af de forespørgsler, den har lavet, de kilder, den har konsulteret, og de ræsonnementstrin, den har taget for at nå sin konklusion. Værktøjer som Azure AI Content Safety og Azure AI Tracing / GenAIOps kan hjælpe med at opretholde gennemsigtighed og reducere risici.
- **Biaskontrol og Balanceret Informationshentning:** Udviklere kan justere hentningsstrategier for at sikre, at balancerede og repræsentative datakilder overvejes, og regelmæssigt gennemgå outputs for at opdage bias eller skæve mønstre ved hjælp af brugerdefinerede modeller til avancerede data science-organisationer, der bruger Azure Machine Learning.
- **Menneskelig Overvågning og Overholdelse:** For følsomme opgaver forbliver menneskelig gennemgang essentiel. Agentic RAG erstatter ikke menneskelig dømmekraft i beslutninger med høj risiko—den supplerer den ved at levere mere grundigt gennemarbejdede muligheder.

At have værktøjer, der giver en klar registrering af handlinger, er afgørende. Uden dem kan det være meget vanskeligt at fejlfinde en flertrinsproces. Se følgende eksempel fra Literal AI (virksomheden bag Chainlit) for en Agent-run:

![AgentRunExample](../../../translated_images/AgentRunExample.471a94bc40cbdc0cd04c1f43c8d8c9b751f10d97918c900e29cb3ba0d6aa4c00.da.png)

![AgentRunExample2](../../../translated_images/AgentRunExample2.19c7410a03bbc216c446b8a4e35ac82f1e8bc0ed313484212f5f4d1137637245.da.png)

## Konklusion

Agentic RAG repræsenterer en naturlig udvikling i, hvordan AI-systemer håndterer komplekse, dataintensive opgaver. Ved at anvende et loop-interaktionsmønster, selvstændigt vælge værktøjer og forfine forespørgsler, indtil der opnås et resultat af høj kvalitet, bevæger systemet sig ud over statisk prompt-følgen og bliver en mere adaptiv, kontekstbevidst beslutningstager. Selvom det stadig er begrænset af menneskedefinerede infrastrukturer og etiske retningslinjer, muliggør disse agentiske evner rigere, mere dynamiske og i sidste ende mere nyttige AI-interaktioner for både virksomheder og slutbrugere.

### Har du flere spørgsmål om Agentic RAG?

Deltag i [Azure AI Foundry Discord](https://aka.ms/ai-agents/discord) for at møde andre lærende, deltage i kontortid og få svar på dine spørgsmål om AI-agenter.

## Yderligere Ressourcer

-
<a href="https://learn.microsoft.com/training/modules/use-own-data-azure-openai" target="_blank">
Implementering af Retrieval Augmented Generation (RAG) med Azure OpenAI Service: Lær hvordan du bruger dine egne data med Azure OpenAI Service. Denne Microsoft Learn-modul giver en omfattende guide til implementering af RAG  
- <a href="https://learn.microsoft.com/azure/ai-studio/concepts/evaluation-approach-gen-ai" target="_blank">Evaluering af generative AI-applikationer med Azure AI Foundry: Denne artikel dækker evaluering og sammenligning af modeller på offentligt tilgængelige datasæt, inklusive Agentic AI-applikationer og RAG-arkitekturer</a>  
- <a href="https://weaviate.io/blog/what-is-agentic-rag" target="_blank">Hvad er Agentic RAG | Weaviate</a>  
- <a href="https://ragaboutit.com/agentic-rag-a-complete-guide-to-agent-based-retrieval-augmented-generation/" target="_blank">Agentic RAG: En komplet guide til agentbaseret Retrieval Augmented Generation – Nyheder fra generation RAG</a>  
- <a href="https://huggingface.co/learn/cookbook/agent_rag" target="_blank">Agentic RAG: boost din RAG med forespørgselsreformulering og selv-forespørgsel! Hugging Face Open-Source AI Cookbook</a>  
- <a href="https://youtu.be/aQ4yQXeB1Ss?si=2HUqBzHoeB5tR04U" target="_blank">Tilføjelse af agentiske lag til RAG</a>  
- <a href="https://www.youtube.com/watch?v=zeAyuLc_f3Q&t=244s" target="_blank">Fremtiden for vidensassistenter: Jerry Liu</a>  
- <a href="https://www.youtube.com/watch?v=AOSjiXP1jmQ" target="_blank">Sådan bygger du Agentic RAG-systemer</a>  
- <a href="https://ignite.microsoft.com/sessions/BRK102?source=sessions" target="_blank">Brug af Azure AI Foundry Agent Service til at skalere dine AI-agenter</a>  

### Akademiske artikler  

- <a href="https://arxiv.org/abs/2303.17651" target="_blank">2303.17651 Self-Refine: Iterativ forfining med selv-feedback</a>  
- <a href="https://arxiv.org/abs/2303.11366" target="_blank">2303.11366 Reflexion: Sproglige agenter med verbal forstærkningslæring</a>  
- <a href="https://arxiv.org/abs/2305.11738" target="_blank">2305.11738 CRITIC: Store sprogmodeller kan selv-korrigere med værktøjsinteraktiv kritik</a>  
- <a href="https://arxiv.org/abs/2501.09136" target="_blank">2501.09136 Agentic Retrieval-Augmented Generation: En undersøgelse af Agentic RAG</a>  

## Forrige lektion  

[Designmønster for værktøjsbrug](../04-tool-use/README.md)  

## Næste lektion  

[Opbygning af troværdige AI-agenter](../06-building-trustworthy-agents/README.md)  

---

**Ansvarsfraskrivelse**:  
Dette dokument er blevet oversat ved hjælp af AI-oversættelsestjenesten [Co-op Translator](https://github.com/Azure/co-op-translator). Selvom vi bestræber os på nøjagtighed, skal du være opmærksom på, at automatiserede oversættelser kan indeholde fejl eller unøjagtigheder. Det originale dokument på dets oprindelige sprog bør betragtes som den autoritative kilde. For kritisk information anbefales professionel menneskelig oversættelse. Vi påtager os intet ansvar for misforståelser eller fejltolkninger, der måtte opstå som følge af brugen af denne oversættelse.