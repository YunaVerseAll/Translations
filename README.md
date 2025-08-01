MTL
- 3 days of testing (models, prompt styles, methods) and stuff and I'm using this method
I only do a little clean up here and there for formatting and stuff cause mtl is inconsistent
But I don't do proof reading, cause I'm not really making these to release but rather for myself
I just happen to be sharing them cause why not, I've already made them, if you don't like them
Well I'm sharing my method so go right on ahead and do it yourself, I'll recommend some improvements at the end
The reason I don't do them myself is cause I'm lazy and don't have the hardware for it

So 
First I find a web novel I wanna translate 
Then I grab a chapter of the novel in plain text
Use an LLM to extract key information, 
Such as Character Names, Place Names, Terms, etc and selectively create a glossary of those words
E.g.
Characters:
季沫 = Ji Mo - Main Character, Cannon Fodder, Keen Senses, Reincarnated Host, Emotionally Resilient, Slave Maid
系统444号 = System 444 - Transmigration System, Cold, Machine Like, Observant, Slightly Sarcastic  
44号宿主 = Host 44 - Alias For of Ji Mo, Exclusively Used By System 444

Locations:
侯府 = Marquis Estate

Terms:
反派 = Antagonist  
投放 = Transmigration
系统 = System  
积分 = Points
系统商城 = System Store
空间袋 = Pocket Dimension
宿主 = Host  
任务 = Task
支线任务 = Side Task
逆袭 = Counterattack
仇女狂 = Misogynist
炮灰 = Cannon Fodder

I repeat this for multiple chapters (ideally I'd do it for all of them but aint nobody got time for that) until I feel like I have enough stuff in the glossary

Using this glossary I add it to a prompt that tells the llm to translate the text I provide using the glossary for consistancy 
And then I just go chapter by chapter translating with that prompt

Fix any glaring issues like inconsistant use of punctuation and untranslated characters, and boom basically done
Sometimes I make corrections on stuff but eh

Now the way I do it is using a low end llm like a 30b quantized one, and a context of 10k so I sometimes have to split the chapters and stuff
If you have the hardware for it, you'd use a better model and higher context, maybe even enough to translate the full arc in one go, not that I'd recommend it since that has it's own problems, but yea, if you have the hardware for it, or have decent hardware and don't mind it taking a lot longer then you can do that
For context I have a 3080 10gb vram gpu and 32gb ram with an i7-12700k processor 
And if I use a 32b model that's good for translating (qwen3-32b) the quality is about 10-20% better and more consistent, but it takes 40~ minutes to translate a chapter at low context (6000-6500) (cause I don't have enough ram for high context) 
And that's just the translation, I did this test before I did glossary creation, so with that included it would probably take 50~ minutes per chapter
To compare the smaller model I'm using makes it so I get a chapter done in about 15 minutes, inclusing glossary created (per chapter so about 4 minutes for the glossary for the chapter and 6-10 minutes for the translation)
So yea for the drop in quality, for say a QT novel I save about 15h per arc, if we assume an arc is 20 chapters long, could I do it that way and improve the quality? Yea. Am I? Nuh uh
The text is designed specifically for TTS cause I use tts to basically listen to the novel like an audiobook by making it into an epub format and passing through something that can tts epubs
