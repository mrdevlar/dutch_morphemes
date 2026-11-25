# Dutch Morpheme Dictionary

## Recommended Usage

Download the repo above (download source), unzip it into a folder or use a git client to clone it. Install [Obsidian](https://obsidian.md/) and select the folder that you unzipped it into as the "Vault Location".
This is recommended because you can use Obsidian search functions to navigate the dictionary rather than just by filename. 

## Web Usage

Just click on the `morphemes` folder above and Github will let you see any markdown files with formatting. No installation needed.

## Mobile Usage on Android with MGit and Obsidian

To use this on Android Mobile, please download [MGit](https://play.google.com/store/apps/details?id=com.manichord.mgit&hl=en-US) and [Obsidian Mobile](https://play.google.com/store/apps/details?id=md.obsidian).
It will allow you to clone the repo and pull any changes.

- Launch MGit, go to the "..." and click "Settings", under "General" Click "Root Storage Location for Repos"
- Then select `Documents`. This is required because MGit, by default, places repos in a location inaccessible by other apps.
- Go back, go to the "+"
- Remote URL: `https://github.com/mrdevlar/dutch_morphemes`
- Local path: `dutch_morphemes`
- Press "Clone"

You'll now have a folder called `dutch_morphemes` in the document folder. You can click on the repo in MGit and press the icon in the top right, and press "pull" to update the morphemes at any time.

- Launch Obsidian
- Go to "Manage Vaults..."
- Click "Open folder as vault"
- Select the `dutch_morphemes` folder in the `Documents`
- Wait for the index to finish building.
- You now have a searchable dictionary on mobile.

## What is this?

It's an English language dictionary of Dutch Morphemes. 

The initial word selection was taken from the fantastic book "Nederlands in Actie" by Berna de Boer, Margaret van der Kamp, Simone Pentermann. But increasingly it is filled with words that interest me. 

## Why do this?

I always wanted to write a dictionary, since I encountered an English one in the 3rd grade and thought was the most amazing item.

The other major reason is because the wonder of Dutch is that the language is compositional. Let me illustrate using my two favorite Dutch words.

First, the Dutch word _handschoenen_ translates into the English word "gloves". It's composed of "hand" which translates into "hand", like the kind with fingers, and "schoenen" which translates into "shoes". So the Dutch word for "gloves" is actually "hand shoes".

Second, the Dutch verb _verwachten_ translates into the English verb to "expect". It's composed to "ver" which means "away from" and "wachten" which means "to wait". So the Dutch word for "expect" is to "away wait".

A large proportion of the Dutch language is put together in this way.

## How was this made?

This was made with an AI model, `unsloth/Qwen3.5-122B-A10B-GGUF`, quantized at `Q4_K_XL`. 

For linguistics, it continues to be an excellent model due to its parameter size that is very clear in its exposition. Better overall models might exist, but this one is preferred for this type of task.

## Errata

If you find something wrong, please open an issue. 

If you want to add more words, please use the previously mentioned model with the prompt:

```commandline
From a linguistic perspective, please break up and explain the morphemes in the Dutch word: "`{word}`"'
```

And submit a PR. 


# License

CC BY-NC-SA 4.0