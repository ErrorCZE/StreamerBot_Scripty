# [Kód pro zpracování soutěží](https://github.com/ErrorCZE/StreamerBot_Scripty/blob/main/Sout%C4%9B%C5%BE.txt)
- Přes příkaz/twitch odměnu/dle vašeho triggeru zapíše po vyzvednutí uživatele do souboru (cestu k souboru si určujete vy)
- Přes příkaz !přihlášení/prihlaseni/... (můžete změnit) to vypíše seznam registrovaných lidí (z dokumentu)
- Do dokumentu se ukládá twitch jméno a twitch id ve formátu `id,jméno`
- Do dokumentu můžete ručně přidávat lidi, ale musíte dodržet velikost písmen v jejich jménu a dávat každého na nový řádek. Místo jejich ID zadejte třeba `00000`
- Do soutěže se lze přihlásit pouze jednou, poté to napíše, že je již přihlášený a vrátí to automaticky body
- Když něco nebude fungovat, tak to do chatu napíše důvod (chybu)... např. že neexistuje soubor, který jste nastavili


# [Kód pro vytváření klipů s odesíláním na discord](https://github.com/ErrorCZE/StreamerBot_Scripty/blob/main/Vytvo%C5%99en%C3%AD%20klipu.txt)
- Přes příkaz/odměnu/streamdeck/... vytvoří klip z posledních 30s
- Při vytváření oznámí do chatu, že vytváří klip a jméno, kdo zadal příkaz pro vytvoření
- Po vytvoření se odešle do chatu zpráva s odkazem na klip a jménem, kdo ho dal vytvořit. Zároveň se to přes webhook odešle na váš discord


# [Kód pro info o zbývajícím cooldownu na příkaz]([https://github.com/ErrorCZE/StreamerBot_Scripty/blob/main/Cooldown%20info](https://github.com/ErrorCZE/StreamerBot_Scripty/blob/main/Cooldown%20info.txt))
- Přidáte si do triggerů jednotlivé Command cooldowny u kterých chcete, aby to oznamovalo info o cooldownu
- Formát zpráv:
`@Jméno, zbývající globální cooldown: 1d 3h 46m 35s`
`@Jméno, tvůj zbývající cooldown: 46m 35s`
(nepíše to 0d 0m atd... nepíše to jednotky, které jsou 0)


# [Kód pro vytvoření předpovědi a vyhodnocení](https://github.com/ErrorCZE/StreamerBot_Scripty/blob/main/P%C5%99edpov%C4%9B%C4%8F%20Ano-Ne.txt)
- Aktuálně nastaveno na "Přežiju?"
- Možné odpovědi: Ano/Ne

# [Kód pro ovládání Tapo led pásku L900](https://github.com/ErrorCZE/StreamerBot_Scripty/tree/main/L900%20TAPO%20Ovl%C3%A1d%C3%A1n%C3%AD)
### POUZE JAKO TWITCH ODMĚNY ZA BODY
**Případné ovládání přes příkazy atd, si musíte udělat ručně s využitím dostupných akcí napsaných níže**

Spouští se .exe soubor, do soubor .txt se stejným názvem jako je .exe vložte údaje
(.exe jde nakopírovat s jinýma názvama a použít na několik zařízeních... Takže např. svetla1.exe + svetla1.txt; svetla2.exe + svetla2.txt)

Ve streamer botovi nastavte cestu k .exe souboru a cestu do složky, kde tento .exe je. (U všech akcí)

Pro odměny, které nastavují nějaké hodnoty (barva přes hex a světlost) nastavte možnost psaní

Hodnoty pro světlost jsou 1 až 100
Barva se zadává pomocí hex kodu např. #0166FG (barva neovlivňuje světlost, musí se nastavit zvlášť)

Při nedodržení podmínek to vrátí body

**Dostupné akce:**
- setcolor
- setbrightness
- turnon
- turnoff

**Příklady pro použití mimo streamer bota:**
- -a setcolor -c `"hue:saturation"` -n
- -a setbrightness -b `hodnota` -n
- -a turnoff -n
- -a turnon
