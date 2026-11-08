# Dutch Morpheme Dictionary

## Recommended Usage

Download the repo above (download source), unzip it into a folder. Install [Obsidian](https://obsidian.md/) and select the folder that you unzipped it into as the "Vault Location".
This is recommended because you can use Obsidian search functions to navigate the dictionary rather than just by filename. 

## Easiest Usage

Just click on the `morphemes` folder above and Github will let you see any markdown files with formatting. No installation needed.

## What is this?

It's an English language dictionary of Dutch Morphemes. 

The initial word selection was taken from the fantastic book "Nederlands in Actie" by Berna de Boer, Margaret van der Kamp, Simone Pentermann. But increasingly it is filled with words that interest me. 

## Why do this?

I always wanted to write a dictionary, since I encountered an English one in the 3rd grade and thought was the most amazing item.

The other major reason is because the wonder of Dutch is that the language is compositional. Let me illustrate using my two favorite Dutch words.

First, the Dutch word _handschoenen_ translates into the English word "gloves". It's composed of "hand" which translates into "hand", like the kind with fingers, and "schoenen" which translates into "shoes". So the Dutch word for "gloves" is actually "hand shoes".

Second, the Dutch verb "verwachten" translates into the English verb to "expect". It's composed to "ver" which means "away from" and "wachten" which means "to wait". So the Dutch word for "expect" is to "away wait".

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