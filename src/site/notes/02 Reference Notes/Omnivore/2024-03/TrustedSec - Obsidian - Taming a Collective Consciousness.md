---
{"dg-publish":true,"permalink":"/02-reference-notes/omnivore/2024-03/trusted-sec-obsidian-taming-a-collective-consciousness/","title":"TrustedSec - Obsidian - Taming a Collective Consciousness\n","metatags":{"description":"A thorough examination on using Obsidian collaboratively with Git","og:image":"https://i.imgur.com/LmCg5HX.png"},"tags":["MMW-Dev/Workflow"]}
---


## TrustedSec - Obsidian - Taming a Collective Consciousness
#Omnivore

[Read on Omnivore](https://omnivore.app/me/trusted-sec-obsidian-taming-a-collective-consciousness-18e56204d1d)
[Read Original](https://www.trustedsec.com/blog/obsidian-taming-a-collective-consciousness)

### Highlights

> Our Obsidian Git configuration consists of the following settings:
> 
> 1. Vault Backup Interval: 60 
> 2. Auto Pull Interval: 10 
> 3. Commit Message: FLast {{date}} 
> 4. Date Placeholder: MM-DD-YYYY HH:mm:ss 
> 5. Pull Changes Before Push: Enabled (default) [⤴️](https://omnivore.app/me/trusted-sec-obsidian-taming-a-collective-consciousness-18e56204d1d#cc1397a0-1e56-4970-bc53-9345a9479ead) 
{ #cc1397a0}


Example Obsidian Git configuration for a collaborative Obsidian project.

> Additionally, since we’re using Git, we were also able to leverage a .gitignore file to omit files and directories which either caused frequent conflicts or we deliberately did not want synced. We ultimately landed on a .gitignore file configuration of:
> 
> .obsidian/*
> 
> 
> .obsidian/workspace/*
> 
> 
> .obsidian/plugins/*
> 
> 
> $VAULTNAME/Personal/
> 05*-*Personal/
> 
> 
> Day*Planners/*
> 
> 
> .obsidian-git-data
> 
> 
> Untitled*
> 
> null*
> 
> 
> .trash/
> .DS_Store [⤴️](https://omnivore.app/me/trusted-sec-obsidian-taming-a-collective-consciousness-18e56204d1d#7309501c-8366-4a7d-b0f2-9928151f537e) 
{ #7309501c}


Example .gitignore configuration for an Obsidian Git workflow.

> #### Templates for Automation
> 
> Using [SilentVoid13's Templater](https://github.com/SilentVoid13/Templater) plugin, I’ve required the association of a Search Tag and a Title on the creation of a note. To require a template to run on the creation of a new note, you need to modify the following settings in the configuration options for the Templater Plugin `Settings > Community Plugins`.
> 
> 1. Template Folder Location
> 
> ![](https://proxy-prod.omnivore-image-cache.app/0x0,sLfpc5lhxF1iZAjocUOYWWYj5hTGuldXJ-ZrZhhioYlw/https://www.trustedsec.com/wp-content/uploads/2021/09/Pasted-image-20210901152630.png)
> 
> 1. Set `Empty file template` to `04 - Templates/0400 - Gen_Note`. Differentiated by markdown "struct" we assign, this note will serve for the basis of _ALL_ notes (content or categories).
> 
> ![](https://proxy-prod.omnivore-image-cache.app/0x0,soqOTxlwGb68wmfgr7YkPQXDKApBwnHK_ZUnBSC_iGJY/https://www.trustedsec.com/wp-content/uploads/2021/09/Pasted-image-20210901152742.png)
> 
> Here we'll assign the Search Tag associated with TTP, and the title should be automatically populated from the link we clicked to create the note.
> 
> ![](https://proxy-prod.omnivore-image-cache.app/0x0,s9l3rsTMIYnOpmSeedH4vZP6KpXmEA9Sv5p-nkg8rLZE/https://www.trustedsec.com/wp-content/uploads/2021/09/Pasted-image-20210901152436.png)
> 
> ![](https://proxy-prod.omnivore-image-cache.app/0x0,s1PTUdbr0yLIPLNCO-dgV5EBKAzpdnqsmaOf9p_MH_Mo/https://www.trustedsec.com/wp-content/uploads/2021/09/Pasted-image-20210901152954.png)
> 
>   
> We created our note successfully! Since we selected the Search Tag of TTP, templater combined markdown elements to "build" a "TTP" note containing the boilerplate metadata and headings that may help a user get started documenting a particular TTP. Using templates in this way facilitates the abstraction of users from the overhead of committing information. In turn, this allows them to focus less on the categorization and organization of data and empowers us to control it administratively. [⤴️](https://omnivore.app/me/trusted-sec-obsidian-taming-a-collective-consciousness-18e56204d1d#3d5edccb-c393-467a-8676-ced8aa1d67a2) 
{ #3d5edccb}


Integrating Templater into the workflow to prepopulate required metadata fields and document structure.

