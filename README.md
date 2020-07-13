# Vizuálna analýza malej fotovoltickej elektrárne s použitím Excelu a Power BI Desktop

Aplikácia využíva Microsoft Excel pre zber dát o prevádzke malej fotovoltaickej elektrárne a Microsoft Power BI Desktop pre tvorbu reportov.

Popis aplikácie nájdete v článku Power BI a vizuálna datová analýza malej fotovoltickej elektrárne - https://www.saeautom.sk/download/FVEandPowerBI.pdf. Príklad reportu v pdf dokumente vytvoreného pomocou Power BI Desktop nájdete na 
https://github.com/SAE-Automation/Photovoltaics_Power_BI/blob/master/FV7.pdf .

Pre využitie aplikácie je potrebné mať naištalovaný Microsoft Excel, napr. poskytovaný v rámci Microsoft 365, a aplikáciu Microsoft Power BI Desktop, ktorú je možné stiahnúť z https://www.microsoft.com/en-us/download/details.aspx?id=45331 . Pred stiahnutím je vhodné nastaviť požadovaný jazyk užívateľského rozhrania - je možné si nastaviť slovenskú verziu.

Na <https://github.com/SAE-Automation/Photovoltaics_Power_BI> nájdete xlsx súbor Fotovoltaika.xlsx s údajmi o prevádzke FVE ako aj šablónu pre vytvorenie Power BI zostavy - súbor s príponou pbit. Po skopírovaní a dvojkliku na pbit-súbor šablóny sa Vám otvorí aplikácia Power BI Desktop. Do dialogového okna, ktoré sa otvorí, je potrebné zadať úplnú cestu k lokalite na Vašom počítači, do ktorej ste si stiahli súbor Fotovoltaika.xlsx (napr. v tvare D:\Photovoltaics_Power_BI\Fotovoltaika.xlsx). Tento spôsob otvárania aplikácie využíva parameter pre Power BI zostavu, do ktorého sa automaticky kopíruje cesta k súboru Fotovoltaika.xlsx. 

Iný spôsob otvárania aplikácie Power BI zostavy (neobsahujúcej patrameter) je popísaný v článku na <https://github.com/SAE-Automation/Photovoltaics_Power_BI/blob/master/FV3.pdf>. 

Pre využitie aplikácie s vlastnými dátami je potrebné data z listu "MesiaceDodávky" v súbore Fotovoltaika.xlsx nahradiť vlastnými dátami pričom pôvodné názvy stlpcov musia zostať nezmenené.

Demo verziu aplikácie generovanej v Power BI Pro a vloženej do webovej aplikácie využívajúcej Blazor WebAssembly na Microsoft Azure lokalite pre statické webové aplikácie môžete spustiť vo webovom prehlíadači na <https://csbf095064e64c6x4f64x886.z6.web.core.windows.net/>. 

Demo aplikácia môže bežať aj samostatne v Power BI cloude - pozrite si na <https://app.powerbi.com/view?r=eyJrIjoiMTQzZTIwZDEtMmY2MS00NjFkLTliMzQtOTkwYzQyNWQ5MGI5IiwidCI6ImNmZjU5MDQ2LTc5MzUtNGU3NS04OGY0LTNjODZjMTc1MTVjYyIsImMiOjl9> .

Je výhodné používať pre zadávanie odpočtov súbor Fotovoltaika.xlsx umiestnený v SharePoint alebo OneDrive adresári. K takemúto súboru je potom možné pristupovať aj z online verzie Excelu na mobile.
Zdroj dat je v takomto prípade definovaný ako  
	Source = Excel.Workbook(Web.Contents(XLSXfileLocation), null, true),
kde parameter XLSXfileLocation môže byť napr. https://saeautomation.sharepoint.com/Zdielane%20dokumenty/Fotovoltaika.xlsx. (Samozrejme je potrebné nahradiť saeautomation.sharepoint.com Vašim sharepoint účtom.)




