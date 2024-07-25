# RT-Extension-SaveDraft

## Leírás
Hozzászólásoknál (Ticket/Update.html) a Richtext editorba írt szöveget a bngészú localstore-ba menti és szükség esetén visszatölti.

#### Tulajdonságok

## RT kompatibilitás
RT 5.0.x

## Telepítés
1. végrehaitani a következő parancsokat
````
cd /opt/rt5/local/plugins
git clone https://github.com/DOCCA-CO/RT-Extension-SaveDraft.git
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
- A lokalizázió nem működik, de nem jöttem rá, mi a baja....
