<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "1e40fe956ff79462a02a17080b125041",
  "translation_date": "2025-08-29T20:01:43+00:00",
  "source_file": "01-intro-to-ai-agents/README.md",
  "language_code": "hu"
}
-->
[![Bevezetés az AI ügynökökbe](../../../translated_images/lesson-1-thumbnail.d21b2c34b32d35bbc7f1b4a40a81b031970b6076b4e0c59fb006cf818cac5d4a.hu.png)](https://youtu.be/3zgm60bXmQk?si=QA4CW2-cmul5kk3D)

> _(Kattints a fenti képre a leckéhez tartozó videó megtekintéséhez)_

# Bevezetés az AI ügynökökbe és azok felhasználási területeibe

Üdvözlünk az "AI ügynökök kezdőknek" kurzuson! Ez a kurzus alapvető ismereteket és gyakorlati példákat nyújt az AI ügynökök létrehozásához.

Csatlakozz a [Azure AI Foundry Discord](https://aka.ms/ai-agents/discord) közösséghez, hogy találkozz más tanulókkal és AI ügynök fejlesztőkkel, valamint feltehesd kérdéseidet a kurzussal kapcsolatban.

A kurzus kezdetén megismerkedünk azzal, hogy mik az AI ügynökök, és hogyan használhatjuk őket az általunk létrehozott alkalmazásokban és munkafolyamatokban.

## Bevezetés

Ez a lecke az alábbiakat tárgyalja:

- Mik azok az AI ügynökök, és milyen típusú ügynökök léteznek?
- Melyek a legjobb felhasználási területek az AI ügynökök számára, és hogyan segíthetnek nekünk?
- Melyek az alapvető építőelemek az ügynöki megoldások tervezésekor?

## Tanulási célok
A lecke elvégzése után képes leszel:

- Megérteni az AI ügynökök koncepcióját, és hogyan különböznek más AI megoldásoktól.
- Hatékonyan alkalmazni az AI ügynököket.
- Produktívan tervezni ügynöki megoldásokat a felhasználók és ügyfelek számára.

## Az AI ügynökök meghatározása és típusai

### Mik azok az AI ügynökök?

Az AI ügynökök olyan **rendszerek**, amelyek lehetővé teszik a **nagy nyelvi modellek (LLM-ek)** számára, hogy **cselekvéseket hajtsanak végre**, azáltal hogy kiterjesztik képességeiket, és hozzáférést biztosítanak számukra **eszközökhöz** és **tudáshoz**.

Bontsuk le ezt a definíciót kisebb részekre:

- **Rendszer** - Fontos, hogy az ügynökökre ne csak egyetlen komponensként gondoljunk, hanem egy több komponensből álló rendszerként. Az AI ügynök alapvető komponensei:
  - **Környezet** - Az a meghatározott tér, ahol az AI ügynök működik. Például, ha egy utazási foglalási AI ügynököt nézünk, a környezet lehet az utazási foglalási rendszer, amelyet az ügynök használ a feladatok elvégzéséhez.
  - **Érzékelők** - A környezet információt és visszajelzést nyújt. Az AI ügynökök érzékelőket használnak, hogy összegyűjtsék és értelmezzék a környezet aktuális állapotáról szóló információkat. Az utazási foglalási ügynök példájában a foglalási rendszer információt nyújthat például a szállodai elérhetőségről vagy repülőjegyárakról.
  - **Végrehajtók** - Miután az AI ügynök megkapja a környezet aktuális állapotát, az ügynök meghatározza, hogy milyen cselekvést hajtson végre a környezet megváltoztatásához. Az utazási foglalási ügynök esetében ez lehet például egy szabad szoba lefoglalása a felhasználó számára.

![Mik azok az AI ügynökök?](../../../translated_images/what-are-ai-agents.1ec8c4d548af601a3a78c6c02e5c355d19c06a4a74fe93e3609a1d08e8c15689.hu.png)

**Nagy nyelvi modellek** - Az ügynökök koncepciója már az LLM-ek létrehozása előtt is létezett. Az AI ügynökök LLM-ekkel való építésének előnye az, hogy képesek értelmezni az emberi nyelvet és adatokat. Ez a képesség lehetővé teszi az LLM-ek számára, hogy értelmezzék a környezeti információkat, és tervet készítsenek a környezet megváltoztatására.

**Cselekvések végrehajtása** - Az AI ügynök rendszereken kívül az LLM-ek korlátozottak olyan helyzetekben, ahol a cselekvés tartalom vagy információ generálása a felhasználó kérésére. Az AI ügynök rendszereken belül az LLM-ek képesek feladatokat végrehajtani, például értelmezni a felhasználó kérését, és használni azokat az eszközöket, amelyek elérhetők a környezetükben.

**Hozzáférés eszközökhöz** - Az, hogy az LLM milyen eszközökhöz fér hozzá, 1) a környezetétől és 2) az AI ügynök fejlesztőjétől függ. Az utazási ügynök példájában az ügynök eszközei korlátozottak lehetnek a foglalási rendszer által elérhető műveletekre, illetve a fejlesztő korlátozhatja az ügynök eszközhozzáférését például csak repülőjáratokra.

**Memória + Tudás** - A memória lehet rövid távú, a felhasználó és az ügynök közötti beszélgetés kontextusában. Hosszú távon, a környezet által nyújtott információn kívül, az AI ügynökök más rendszerekből, szolgáltatásokból, eszközökből és akár más ügynököktől is tudást szerezhetnek. Az utazási ügynök példájában ez a tudás lehet például a felhasználó utazási preferenciáira vonatkozó információ, amely egy ügyféladatbázisban található.

### Az ügynökök különböző típusai

Most, hogy van egy általános definíciónk az AI ügynökökről, nézzük meg néhány konkrét ügynöktípust, és hogyan alkalmazhatók egy utazási foglalási AI ügynöknél.

| **Ügynöktípus**               | **Leírás**                                                                                                                           | **Példa**                                                                                                                                                                                                                   |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Egyszerű reflex ügynökök**  | Azonnali cselekvéseket hajtanak végre előre meghatározott szabályok alapján.                                                          | Az utazási ügynök értelmezi az e-mail tartalmát, és továbbítja az utazási panaszokat az ügyfélszolgálatnak.                                                                                                                  |
| **Modellalapú reflex ügynökök** | A világ modellje és annak változásai alapján hajtanak végre cselekvéseket.                                                            | Az utazási ügynök prioritást ad az útvonalaknak, ahol jelentős árváltozások történtek, a történelmi áradatokhoz való hozzáférés alapján.                                                                                       |
| **Célalapú ügynökök**         | Terveket készítenek konkrét célok elérésére, értelmezve a célt, és meghatározva a szükséges cselekvéseket annak eléréséhez.            | Az utazási ügynök lefoglal egy utazást, meghatározva a szükséges utazási intézkedéseket (autó, tömegközlekedés, repülőjáratok) a jelenlegi helyszíntől a célállomásig.                                                          |
| **Hasznosságalapú ügynökök**  | Figyelembe veszik a preferenciákat, és számszerűen mérlegelik a kompromisszumokat a célok eléréséhez.                                 | Az utazási ügynök maximalizálja a hasznosságot, mérlegelve a kényelmet és a költségeket az utazás foglalásakor.                                                                                                               |
| **Tanuló ügynökök**           | Idővel javulnak, visszajelzésekre reagálva és cselekvéseiket ennek megfelelően módosítva.                                             | Az utazási ügynök javítja teljesítményét az ügyfél visszajelzései alapján, például utazás utáni kérdőívek segítségével, hogy a jövőbeni foglalásoknál jobb döntéseket hozzon.                                                  |
| **Hierarchikus ügynökök**     | Többszintű rendszert alkotnak, ahol a magasabb szintű ügynökök feladatokat bontanak le alacsonyabb szintű ügynökök számára.           | Az utazási ügynök lemond egy utazást, a feladatot részfeladatokra bontva (például konkrét foglalások törlése), és az alacsonyabb szintű ügynökök végrehajtják ezeket, majd visszajelzést adnak a magasabb szintű ügynöknek.       |
| **Több ügynökből álló rendszerek (MAS)** | Az ügynökök önállóan végzik el a feladatokat, akár együttműködve, akár versengve.                                                  | Együttműködő: Több ügynök foglal konkrét utazási szolgáltatásokat, például szállodákat, repülőjáratokat és szórakozási lehetőségeket. Versengő: Több ügynök kezeli és verseng egy közös szállodai foglalási naptárban az ügyfelek elhelyezéséért. |

## Mikor használjunk AI ügynököket?

Az előző szakaszban az utazási ügynök példáját használtuk, hogy bemutassuk, hogyan alkalmazhatók az ügynökök különböző típusai az utazási foglalás különböző forgatókönyveiben. Ezt az alkalmazást a kurzus során továbbra is használni fogjuk.

Nézzük meg, milyen típusú felhasználási esetekben érdemes AI ügynököket alkalmazni:

![Mikor használjunk AI ügynököket?](../../../translated_images/when-to-use-ai-agents.54becb3bed74a479f5caca9c951132ce81d482a6704bcd22e5a600dbabc9434e.hu.png)

- **Nyitott végű problémák** - lehetővé teszik az LLM számára, hogy meghatározza a szükséges lépéseket egy feladat elvégzéséhez, mivel ez nem mindig kódolható előre egy munkafolyamatba.
- **Többlépcsős folyamatok** - olyan feladatok, amelyek bizonyos szintű összetettséget igényelnek, és az AI ügynöknek eszközöket vagy információkat kell használnia több lépésben, nem csak egyszeri lekérdezés során.
- **Idővel történő javulás** - olyan feladatok, ahol az ügynök visszajelzést kap a környezetétől vagy a felhasználóktól, hogy idővel jobb eredményeket nyújtson.

Az AI ügynökök használatának további szempontjait a "Megbízható AI ügynökök építése" leckében tárgyaljuk.

## Az ügynöki megoldások alapjai

### Ügynökfejlesztés

Az AI ügynök rendszer tervezésének első lépése az eszközök, cselekvések és viselkedések meghatározása. Ebben a kurzusban az **Azure AI Agent Service** használatára összpontosítunk az ügynökök definiálásához. Ez olyan funkciókat kínál, mint:

- Nyílt modellek kiválasztása, például OpenAI, Mistral és Llama
- Licencelt adatok használata olyan szolgáltatóktól, mint a Tripadvisor
- Standardizált OpenAPI 3.0 eszközök használata

### Ügynöki minták

Az LLM-ekkel való kommunikáció promptokon keresztül történik. Az AI ügynökök félig autonóm természete miatt nem mindig lehetséges vagy szükséges manuálisan újrapromptolni az LLM-et a környezet változása után. **Ügynöki mintákat** használunk, amelyek lehetővé teszik az LLM promptolását több lépésben, skálázhatóbb módon.

Ez a kurzus néhány jelenleg népszerű ügynöki mintát tárgyal.

### Ügynöki keretrendszerek

Az ügynöki keretrendszerek lehetővé teszik a fejlesztők számára, hogy ügynöki mintákat valósítsanak meg kóddal. Ezek a keretrendszerek sablonokat, bővítményeket és eszközöket kínálnak az AI ügynökök jobb együttműködéséhez. Ezek az előnyök jobb megfigyelhetőséget és hibakeresési lehetőségeket biztosítanak az AI ügynök rendszerek számára.

Ebben a kurzusban megvizsgáljuk a kutatás-orientált AutoGen keretrendszert és a gyártásra kész Agent keretrendszert a Semantic Kernelből.

### További kérdéseid vannak az AI ügynökökről?

Csatlakozz a [Azure AI Foundry Discord](https://aka.ms/ai-agents/discord) közösséghez, hogy találkozz más tanulókkal, részt vegyél konzultációkon, és választ kapj az AI ügynökökkel kapcsolatos kérdéseidre.

## Előző lecke

[Kurzus beállítása](../00-course-setup/README.md)

## Következő lecke

[Ügynöki keretrendszerek felfedezése](../02-explore-agentic-frameworks/README.md)

---

**Felelősség kizárása**:  
Ez a dokumentum az AI fordítási szolgáltatás, a [Co-op Translator](https://github.com/Azure/co-op-translator) segítségével lett lefordítva. Bár törekszünk a pontosságra, kérjük, vegye figyelembe, hogy az automatikus fordítások hibákat vagy pontatlanságokat tartalmazhatnak. Az eredeti dokumentum az eredeti nyelvén tekintendő hiteles forrásnak. Kritikus információk esetén javasolt professzionális emberi fordítást igénybe venni. Nem vállalunk felelősséget semmilyen félreértésért vagy téves értelmezésért, amely a fordítás használatából eredhet.