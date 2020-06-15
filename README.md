# Git på skånska

## Introduktion

Det dagliga språket för de olika kommandona i `git` (eller `fubbick`) är
på skånska ett enda stort skångelskakalas. Jag finner mig själv ofta
sägandes _"Kan du pusha branchen?"_ eller _"Jag pullar!"_.

Detta dokument ämnar etablera en rent skånsk jargong som kan användas
på arbetsplatsen för att med fördel undvika pressade situationer.

## Förslag

Nedan följer tabeller över verb och substantiv relaterade till git,
deras nuvarande bruk samt förslag på hur vi tillsammans kan bättra
oss.

| Verb        | Nuvarande bruk | Förslag       |
|-------------|----------------|---------------|
| init        | inita          | jubba         |
| clone       | klona          | abekatta      |
| pull        | pulla          | asa           |
| push        | pusha          | prega         |
| fetch       | fetcha         | pela          |
| branch      | brancha        | spåga         |
| add         | adda           | åsso          |
| commit      | commita        | hutta         |
| rebase      | rebasa         | nimma         |
| merge       | merga          | klydda        |
| stash       | stasha         | tocka         |
| cherry-pick | cherry-picka   | pela päror    |
| blame       | blamea         | gaffla        |
| checkout    | checka ut      | henka         |
| ammend      | ammenda        | mecka         |
| squash      | squasha        | pannkaga      |

| Substantiv   | Nuvarande bruk | Förslag     |
|--------------|----------------|-------------|
| git          | git            | fubbick     |
| repository   | repo           | hodda       |
| branch       | branch         | spåga       |
| commit       | commit         | drös        |
| pull request | pull request   | jidder      |
| stash        | stash          | tocka       |
| head         | headen         | hue         |
| remote       | remoten        | ude         |
| origin       | origin         | himma       |
| master       | mastern        | kagehus     |
| dev          | deven          | glytt       |

| Attribut   | Nuvarande bruk | Förslag   |
|------------|----------------|-----------|
| force      | force          | mans-     |


## Exempel

    - Kan du asa spågan jag just nimmade och prega den till github?

    - Jag spågade alldeles nyss och hutta ändringarna från min tocka där.

    - Skicka en jidder när du är färdig med klyddandet!

    - Låt oss pela päror från kagehus-spågan.

    - Hoppsan, jag råkade visst fedeprega mot kagehuset. D:

    - Jag har en drös på glytt, kan jag klydda in det i kagehuset och sedan prega himm det?

    - Nils! Du kan inte hutta och prega innan du har asat himm från kagehuset! Nu har pågarna fått en rälig klyddkonflikt!
    
    - Jag brukar alltid hutta till en pågåendejubb-drös som jag meckar innan jag mans-pregar upp det till en spåga. Sen tycker jag att man kan asa nimma innan man pannkageklyddar spågan

## Exempel kommandon

```bash
# git init
fubbick jubba

# git add test.py
fubbick åsso test.py

# git commit -m "Add new features"
fubbick hutta -m "Mög"

# git remote add origin
fubbick ude åsso himma

# git push origin master
fubbick prega himma kagehus

# git pull origin
fubbick asa himma

# git merge origin/dev
fubbick klydda himma/glytt
```

## Dagligt bruk

Nedan följer en rad kommandoradskommandon för att sätta upp en skånsk
gitmiljö. Avsaknaden av skånska tecken i täcknamnen beror på en brist i git
(överväg att förbättra mjukvaran och skicka en jidder!). Följande
kommandon ändrar din `~/.gitconfig` och kommer att verka globalt.

```bash
git config --global alias.jubba init
git config --global alias.abekatta clone
git config --global alias.asa pull
git config --global alias.prega push
git config --global alias.fedeprega "push --force"
git config --global alias.pela fetch
git config --global alias.spaga branch
git config --global alias.asso add
git config --global alias.hutta commit
git config --global alias.nimma rebase
git config --global alias.klydda merge
git config --global alias.tocka stash
git config --global alias.pelaparor cherry-pick
git config --global alias.gaffla blame
git config --global alias.henka checkout

alias fubbick=git
```
