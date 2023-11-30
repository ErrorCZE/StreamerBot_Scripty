# [Kód pro zpracování soutěží](https://github.com/ErrorCZE/StreamerBot---Kody/blob/main/Sout%C4%9B%C5%BE)
- Přes příkaz/twitch odměnu/dle vašeho triggeru zapíše po vyzvednutí uživatele do souboru (cestu k souboru si určujete vy)
- Přes příkaz !přihlášení/prihlaseni/... (můžete změnit) to vypíše seznam registrovaných lidí (z dokumentu)
- Do dokumentu se ukládá twitch jméno a twitch id ve formátu `id,jméno`
- Do dokumentu můžete ručně přidávat lidi, ale musíte dodržet velikost písmen v jejich jménu a dávat každého na nový řádek. Místo jejich ID zadejte třeba `00000`
- Do soutěže se lze přihlásit pouze jednou, poté to napíše, že je již přihlášený a vrátí to automaticky body
- Když něco nebude fungovat, tak to do chatu napíše důvod (chybu)... např. že neexistuje soubor, který jste nastavili


# [Kód pro vytváření klipů s odesíláním na discord](https://github.com/ErrorCZE/StreamerBot---Kody/blob/main/Vytvo%C5%99en%C3%AD%20klipu)
- Přes příkaz/odměnu/streamdeck/... vytvoří klip z posledních 30s
- Při vytváření oznámí do chatu, že vytváří klip a jméno, kdo zadal příkaz pro vytvoření
- Po vytvoření se odešle do chatu zpráva s odkazem na klip a jménem, kdo ho dal vytvořit. Zároveň se to přes webhook odešle na váš discord

# [Kód pro info o zbývajícím cooldownu na příkaz](https://github.com/ErrorCZE/StreamerBot---Kody/blob/main/Cooldown%20info)
- Přidáte si do triggerů jednotlivé Command cooldowny u kterých chcete, aby to oznamovalo info o cooldownu
- Formát zpráv:
`@Jméno, zbývající globální cooldown: 1d 3h 46m 35s`
`@Jméno, tvůj zbývající cooldown: 46m 35s`
(nepíše to 0d 0m atd... nepíše to jednotky, které jsou 0)
