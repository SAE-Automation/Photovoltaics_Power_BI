# Vizuálna analýza malej fotovoltickej elektrárne s použitím Excelu a Power BI Desktop

Aplikácia využíva Microsoft Excel pre zber dát o prevádzke malej fotovoltaickej elektrárne a Microsoft Power BI Desktop pre tvorbu reportov.
Popis aplikácie nájdete v článku Power BI a vizuálna datová analýza malej fotovoltickej elektrárne - https://www.saeautom.sk/download/FVEandPowerBI.pdf. Príklad reportu v pdf dokumente vytvoreného pomocou Power BI Desktop nájdete na  
https://github.com/SAE-Automation/Photovoltaics_Power_BI/blob/master/FV3.pdf .

Pre využitie aplikácie je potrebné mať naištalovaný Microsoft Excel, napr. poskytovaný v rámci Microsoft 365 a aplikáciu Microsoft Power BI Desktop, ktorú je možné stiahnúť si z https://www.microsoft.com/en-us/download/details.aspx?id=45331 . Pred stiahnutím je vhodné nastaviť požadovaný jazyk užívateľského rozhrania - je možné si nastaviť slovenskú verziu.

Na https://github.com/SAE-Automation/Photovoltaics_Power_BI nájdete xlsx súbory s údajmi o prevádzke FVE ako aj šablónu pre vytvorenie Power BI zostavy - súbor s príponou pbit. Po skopírovaní a dvojkliku na pbit-súbor sa Vám otvorí aplikácia Power BI Desktop, ktorá sa pokúsi otvoriť súbor z pôvodného umiestnenia (D:\MsDev\2020\Photovoltaics_Power_BI\Fotovoltaika.xlsx), čo sa mu asi nepodarí, keďže ste si súbory stiahli pravdepodobne do iného umiestnenia. 

Pre nastavenie cesty k Vašim súborom prejdite v Microsoft Power BI Desktop na Editor Power Query (v Sk verzii "Transformovať údaje") a na pravej
strane pod nápisom "Použité kroky" urobte dvojklik na nápis Source. Otvorí sa Vám dialógový box, pomocou ktorého môžete zmeniť cestu k xlsx súboru.

Pre využitie aplikácie s vlastnými dátami je potrebné data z listu "MesiaceDodávky" v súbore Fotovoltaika.xlsx nahradiť vlastnými dátami pričom pôvodné názvy stlpcov musia zostať nezmenené.




