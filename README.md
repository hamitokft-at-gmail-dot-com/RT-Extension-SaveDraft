# RT-Extension-SaveDraft

## Leírás
Hozzászólásoknál (Ticket/Update.html) a Richtext editorba írt szöveget a böngésző localstore-ba menti és szükség esetén visszatölti.

#### Tulajdonságok

## RT kompatibilitás
RT 5.0.x

## Telepítés
1. végrehaitani a következő parancsokat
````
cd /opt/rt5/local/plugins
git clone https://github.com/hamitokft-at-gmail-dot-com/RT-Extension-SaveDraft
````
2. az  /opt/rt5/etc/RT_SiteConfig.pm fájlba beírni
````
Plugin('RT::Extension::SaveDraft');
````
3. törölni a mason cache-t
````
rm -rf /opt/rt5/var/mason_data/obj
````
4. újraindítani a web szervert.

### TODO
- A ticket and transaction részben a select váltást nem követi.....
- Az modal overlay-e mögött aktív marad a main menü, és ezen nem könnyű segíteni az RT-be történő
beleírás nélkül, a z-index állítgatás nem oldja meg a stacking context kezlés miatt.
