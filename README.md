# RT-Extension-SaveDraft

- [RT-Extension-SaveDraft](#rt-extension-savedraft)
  - [Leírás](#leírás)
  - [Tulajdonságok](#tulajdonságok)
    - [RT kompatibilitás](#rt-kompatibilitás)
    - [Nyelvek](#nyelvek)
  - [A telepítés lépései](#a-telepítés-lépései)

## Leírás

Hozzászólásoknál (Ticket/Update.html) a felhsználó által megadott adatokat, szöveget a böngésző localstore-jába menti és a következő oldalbetöltésnél modal-t jelenít meg, ahol az elmentett adatok
kezelhetőek. A hozzászólásokat megkülönbözteti a hibajegy száma, a hozzászólás típua és az idézés típusa szerint és ennek megfelelően tárolja. A tárolt piszkozatokat a hozzászólás elküldésével vagy a modal-on keresztül lehet törölni.

## Tulajdonságok

### RT kompatibilitás

RT 5.0.x

### Nyelvek

- magyar
- angol

## A telepítés lépései

- a repository klónozása

```shell
cd /opt/rt5/local/plugins
git clone https://github.com/hamitokft-at-gmail-dot-com/RT-Extension-SaveDraft
```

- a plugin regisztrációja

```shell
echo 'Plugin('RT::Extension::SaveDraft');' >> /opt/rt5/etc/RT_SiteConfig.pm
```

- a mason obnect cache törlése

```shell
rm -rf /opt/rt5/var/mason_data/obj
```

- A web szerver újraindítása
