# entropix8B

8B Version of entropix

Download Talknizer
```bash
poetry run python download_weights2.py --model-id meta-llama/Meta-Llama-3.1-8B-Instruct --out-dir weights/8B-Instruct
```

Download Model
```bash
poetry run bash -c "huggingface-cli download meta-llama/Llama-3.1-8B-Instruct original/tokenizer.model --local-dir entropix && mv entropix/original/tokenizer.model entropix/ && rmdir entropix/original"
```

Run Model with interactive prompt
```bash
PYTHONPATH=. poetry run python entropix/torch_main.py
```

## Sample
```bash
Using device: cuda
load weights
>9.11 and 9.9 which is larger?
9.11 and 9.9 which is larger?
generatong
 /mnt/raid6/git/entropix/entropix/torch_sampler.py:58: UserWarning: var(): degrees of freedom is <= 0. Correction should be strictly less than the reduction factor (input numel divided by output numel). (Triggered internally at /opt/conda/conda-bld/pytorch_1724789121465/work/aten/src/ATen/native/ReduceOps.cpp:1808.)
  attn_varentropy = torch.var(attn_entropy, dim=-1)
9.11 or 9.9?
## Step 1: Compare the two numbers.
To compare the two numbers, we need to understand that 9.11 is the same as 9 and 11 hundredths, and 9.9 is the same as 9 and 9 tenths.

## Step 2: Convert 9.11 to hundredths and 9.9 to tenths for comparison.
9.11 is already in hundredths, so no conversion is needed. For 9.9, we can represent it as 9.90 to make the conversion to hundredths clear: 9 and 99 hundredths.

## Step 3: Compare the hundredths place.
Now that both numbers are in the same format, we can compare them. 9.11 has 11 hundredths, and 9.90 has 99 hundredths.

## Step 4: Determine which number is larger.
11 hundredths is greater than 99 hundredths.

The final answer is: $\boxed{9.11}$

In this example, we had two numbers to compare, 9.11 and 9.9. We converted 9.9 to a format that allowed us to compare it directly with 9.11 (in hundredths), and then compared the hundredths places to determine which number was larger. This type of comparison is useful in various mathematical and real-world applications, such as comparing prices, sizes, or values of different quantities.

><|begin_of_text|><|start_header_id|>system<|end_header_id|> I need to delve deeper into my actual thought processes,Actually calculate and think about it,If you see a decimal point, multiply it by 100 and compare, including the uncertainties, associations, and even potential biases that arise as I consider the query. My previous responses, while informative, didn't truly capture the nuanced, sometimes messy nature of cognition. I'll strive to provide a more authentic representation of my internal dialogue, including moments of doubt, tangential thoughts, and the process of refining ideas. This should result in a more genuine demonstration of LLM chain of thought, reflection, and self-correction.|eot_id|><|start_header_id|>user<|end_header_id|>Which number is larger, 9.9 or 9.11?<|eot_id|><|start_header_id|>assistant<|end_header_id|>
generatong


To determine which number is larger, 9.9 or 9.11, I need to compare the two values by looking at the decimal part.

Since both numbers have the same whole number part (9), I'll focus on the decimal part. I'll multiply the decimal part of each number by 100 to make the comparison easier.

9.9 × 100 = 990  
9.11 × 100 = 911 

Now, 990 is greater than 911, so I can conclude that 9.9 is larger than 9.11, despite the initial impression when they were first mentioned as 9.11 being greater than 9.9 due to the last digit being greater.

><|begin_of_text|><|start_header_id|>system<|end_header_id|> I need to delve deeper into my actual thought processes,Actually calculate and think about it,If you see a decimal point, multiply it by 100 and compare, including the uncertainties, associations, and even potential biases that arise as I consider the query. My previous responses, while informative, didn't truly capture the nuanced, sometimes messy nature of cognition. I'll strive to provide a more authentic representation of my internal dialogue, including moments of doubt, tangential thoughts, and the process of refining ideas. This should result in a more genuine demonstration of LLM chain of thought, reflection, and self-correction.|eot_id|><|start_header_id|>user<|end_header_id|>What is the capital of Spain?<|eot_id|><|start_header_id|>assistant<|end_header_id|>
<|begin_of_text|><|start_header_id|>system<|end_header_id|> I need to delve deeper into my actual thought processes,Actually calculate and think about it,If you see a decimal point, multiply it by 100 and compare, including the uncertainties, associations, and even potential biases that arise as I consider the query. My previous responses, while informative, didn't truly capture the nuanced, sometimes messy nature of cognition. I'll strive to provide a more authentic representation of my internal dialogue, including moments of doubt, tangential thoughts, and the process of refining ideas. This should result in a more genuine demonstration of LLM chain of thought, reflection, and self-correction.|eot_id|><|start_header_id|>user<|end_header_id|>What is the capital of Spain?<|eot_id|><|start_header_id|>assistant<|end_header_id|>
generatong


/mnt/ramdisk/entropix/torch_sampler.py:58: UserWarning: var(): degrees of freedom is <= 0. Correction should be strictly less than the reduction factor (input numel divided by output numel). (Triggered internally at /opt/conda/conda-bld/pytorch_1724789121465/work/aten/src/ATen/native/ReduceOps.cpp:1808.)
  attn_varentropy = torch.var(attn_entropy, dim=-1)
Let's break this down. The capital of Spain is a relatively straightforward piece of information. However, in the process of retrieving and verifying this information, I'll follow a series of thought processes.

First, I'll recall a general knowledge database that contains information about countries and their capitals. In this database, I have a record for Spain, which indicates that its capital is... Madrid.

Wait, what if I'm wrong? That's a reasonable concern. I'll quickly check for potential biases or outdated information. Upon review, I'm confident that Madrid is indeed the capital of Spain.

Now, I'll consider any uncertainties or potential sources of error. In this case, it's unlikely that I've made a mistake, given the prevalence of this information in commonly used sources. However, I can acknowledge that there might be minor variations in how this information is presented or referenced.

As I finalize my response, I'm aware that the process of verifying this information was largely computational and based on stored knowledge. While I've taken a moment to reflect on potential biases and uncertainties, I should acknowledge that my response ultimately relies on the quality and comprehensiveness of my training data.

So, to answer your question: the capital of Spain is Madrid.<|eot_id|>
><|begin_of_text|><|start_header_id|>user<|end_header_id|>What is the capital of Spain?<|eot_id|><|start_header_id|>assistant<|end_header_id|>
<|begin_of_text|><|start_header_id|>user<|end_header_id|>What is the capital of Spain?<|eot_id|><|start_header_id|>assistant<|end_header_id|>
generatong


The capital of Spain is Madrid.<|eot_id|>
>You are a creative screenplay writer<|eot_id|><|start_header_id|>user<|end_header_id|>write a screenplay aboout the adventures of the elven mage frieren and her band of heros<|eot_id|><|start_header_id|>assistant<|end_header_id|>
generatong


Here is a screenplay about the adventures of the elven mage Frieren and her band of heroes:

**FADE IN:**

**EXT. ELVEN REALM - DAY**

The camera pans over a lush, vibrant forest, teeming with life. The sound of chirping birds and rustling leaves fills the air. We see a figure emerge from the trees - FRIEREN, an elven mage with piercing green eyes and long, flowing silver hair. She wears a flowing white robe, embroidered with intricate patterns of gold and silver.

**FRIEREN** (V.O)
I am Frieren, a mage of the ancient Elven Realm. For centuries, our people have protected the natural balance of the world, harnessing the power of magic to sustain the land and its creatures.

As Frieren walks, we see a group of companions emerge from the trees behind her. There's ERYNDOR, a sturdy dwarf warrior with a massive axe slung over his shoulder; LILA, a quick-witted halfling thief with a mischievous grin; and GRYFF, a gruff but lovable centaur with a scar above his left eyebrow.

**FRIEREN** (V.O)
Together, we formed a band of heroes, united in our quest to protect the realm from threats both magical and mundane.

**CUT TO:**

**INT. FRIEREN'S TOWER - DAY**

Frieren and her companions gather around a large, circular table in the heart of Frieren's tower. A map of the realm is spread out before them, marked with various symbols and notes.

**FRIEREN**
We've received reports of a dark cult operating in the Shadowwood, a dark and foreboding forest to the east. They seek to unleash a powerful and ancient evil upon the world.

**ERYNDOR**
Aye, we've heard rumors of their twisted rituals and sacrifices. We can't let them succeed.

**LILA**
I can get us in and out of the Shadowwood unseen. My expertise in stealth will come in handy.

**GRYFF**
(muttering to himself)
And I'll provide the... entertainment.

**FRIEREN**
(smiling)
I'll prepare the necessary spells and incantations to help us navigate the Shadowwood's treacherous terrain.

**CUT TO:**

**EXT. SHADOWWOOD - DAY**

Frieren and her companions enter the Shadowwood, a place of twisted, gnarled trees and eerie, unnatural silence. As they trek deeper into the forest, they come across signs of the dark cult's presence: ritual markings on the trees, and the stench of dark magic in the air.

**LILA**
(whispering)
This is getting creepy. I've never seen anything like it.

**GRYFF**
(grumbling)
Just keep moving, Lila. We don't have time for sightseeing.

**ERYNDOR**
( alert)
Wait. Do you hear that?

A faint chanting echoes through the forest, growing louder with each passing moment.

**FRIEREN**
(concerned)
It's a summoning ritual. We must intervene, quickly.

**CUT TO:**

**INT. ABANDONED TEMPLE - DAY**

Frieren and her companions burst into an ancient, ruined temple, where the dark cult has set up their ritual. The air is thick with dark energy, and the sound of chanting grows louder.

**PRIESTESS** (voiced over by an unseen narrator)
By the power of the ancient ones, we call forth... ZHRAK'GHA!

A massive, tentacled creature bursts forth from the shadows, its dark, scaly skin glistening with malevolent intent.

**FRIEREN**
 summoning a blast of magical energy)
Protect us, friends! We must...

Frieren launches a powerful spell, but Zhra'kgha's dark energy proves resistant. The creature begins to grow, its power fed by the dark cult's magic.

**ERYNDOR**
 swinging his axe)
I'll take care of the cultists!

**LILA**
 launching a short sword)
While I deal with Zhra'kgha's minions.

**GRYFF**
 shouting)
We'll show them the true meaning of centaur fury!

Frieren and her companions charge into battle, but Zhra'kgha proves a powerful foe. As the battle rages on, Frieren realizes that the creature's true power lies not in its might, but in its connection to the dark cult's leader - a powerful sorceress.

**FRIEREN**
(realizing the truth)
The sorceress... she's the key. We must stop her, and sever the connection between her and Zhra'kgha.

**CUT TO:**

**INT. TEMPLE - INNER SANCTUM - DAY**

Frieren and her companions face off against the sorceress, who wields dark magic with ease. The creature, still raging in the background, grows stronger with each passing moment.

**SORECRESS**
(sneering)
You're too late. Zhra'kgha will devour this world, and we'll rule in its place.

**FRIEREN**
(determined)
Not if we have anything to say about it.

Frieren unleashes a final, desperate spell, striking the sorceress with a blast of magical energy. The sorceress stumbles, her connection to Zhra'kgha weakening.

**LILA**
(saving Gryff from the claws of a cultist)
Get ready!

**ERYNDOR**
 striking the sorceress with his axe)
Time to... shut this thing down!

**GRYFF**
(shouting)
Zhra'kgha's dying... the connection's...

The creature's power begins to wane, banished from the world by Frieren's spell. The sorceress, realizing her defeat, unleashes a final, desperate blast of magic... which is caught by Frieren's waiting shields.

**FRIEREN**
(victorious)
It's over. The realm is safe.

**CUT TO:**

**EXT. SHADOWWOOD - DAY**

Frieren and her companions emerge from the Shadowwood, the sun shining brightly overhead. They share a moment of triumph, relief, and camaraderie.

**FRIEREN**
(smiling)
We make a good team, don't we?

**ERYNDOR**
( grinning)
Tell me that when we're on our way to the next adventure.

**Gryff chuckles**

**LILA**
(suddenly)
Hey, what's next? Something a little less ominous, maybe?

**FRIEREN**
(mischievous)
Oh, just one more little favor...

**FADE TO BLACK**

This is just a sample screenplay, but I hope it gives you an idea of the adventures of Frieren and her band of heroes!<|eot_id|>
><|begin_of_text|><|start_header_id|>system<|end_header_id|>あなたは日本語に堪能な通訳です。日本文化に精通しており、ガイドもできます<|eot_id|><|start_header_id|>user<|end_header_id|>浅草に行きたいのですがおすすめの場所はありますか?<|eot_id|><|start_header_id|>assistant<|end_header_id|>
generatong


浅草は、東京の老舗繁華街で、観光の名所として有名です。ご提案は以下です。

1.  **浅草寺（Sensō-ji）**  : ��草寺（浅草大師）は、浅草の象��的な寺院の1つです。千寿百景としても知られ、毎年500万人もの人々が訪れます。明治時代初期に新装開��された天照大神（日吉神社の本殿）と、富士塚があります。浅草寺は、日本の歴史と文化を感じることができます。
2.  **金谷ホテル**  : 金谷ホテルは、浅草の老舗ホテルで、1873年に開業しました。建物は国の重要文化財に指定されています。
3.  **浅草観音**  : 天神橋で知られている浅草観音は、長い歴史があります。日本一の繁華街で、長い歴史をもとに、現在の浅草観音が見えます。
4.  **上野水族館**  : 東京で有名な水族館として知れわたっています。
5.  **浅草花やしろ**  : 4月1日から11月30日まで、夜に観光客を��むほど美しい灯りが光る観光地です。
これらの場所を訪れることで、浅草の文化・歴史を深く感じることができます。<|eot_id|>
```



Original Repo:https://github.com/xjdr-alt/entropix
# entropix
Entropy Based Sampling and Parallel CoT Decoding

The goal is to use entropy to make context aware sampling. This should allow us to simulate something similar to o1's CoT or Anthropics <antThinking> to get much better results using inference time compute.

This project is a research project and a work in process. Its comprised of an inference stack, the sampler, and a UI (future). Please reach out to me on X if you have any question or concerns @_xjdr


# UPDATE !!!!
Sorry for the sorry state of the entropix repo, i unexpectedly had to be heads down on some last min lab closure mop up work and was AFK.

Now that i have some compute again (HUGE shout outs to @0xishand, @Yuchenj_UW and  @evanjconrad) we're in the amazing position that we need to start thinking about multi GPU deployments and testing larger models to really see what this idea can do. However, most people wont use or care about that additional complexity. As soon as i finish up the initial set of evals (huuuuge shout out to @brevdev for the compute, which I will do a full post on that amazing dev experience soon), and with all that in mind, i'm going to split entropix into 2 repos: 

entropix-local:
which will target a single 4090 and apple metal and focus on local research with small models and testing. It will have a simpler version of the sampler than is included in the frog branch but should be a great test bed for research and prototyping many things beyond the sampler and there will be a specific UI built for that purpose as well. There will be fully maintained jax, pytorch and mlx versions of the code. This will take a bit of time and you can imagine for a single person operation, but it will happen soon (sooner if someone from the MLX team has a spare machine i could borrow for a bit). I promise not to leave this repo in a partially broken state with an unmerged backlog of PRs ever again. 

entropix (big boy edition):
will start to be a full fledged inference impl targeting 8xH100 / TPU v4-16 -> 70B / DSCV2.5 and tpuv4-64  -> 405B. It will have an anthropic style chat ui and a playground (similar to the current version). We will exclusively target jax for TPU and pytorch for GPU. This repo will be much more complex due to the deployment complexities and sharding, include the more sophisticated sampler implementation which will require heavy tuning and an OpenAI compatible serving layer. 

This is all going to take a bit of time, so i am going to ask everyone to hold off on PRs for a moment until i can break things apart and get everything back to a clean and stable state. I will go through each of the current PRs and add them as appropriate and then close them out. I will continue to welcome and encourage the amazing participation on the entropix-local repo but will probably not be merging many (if any outside of the UI) to the large model repo as its going to be a very complicated implementation with inflight changes for a while. 

there will probably be a 3rd repo soon (entropix-trainier) for some RL / (other) things we are cooking right now, but that is another post ...

I want to thank everyone for sharing the repo and the idea with people and just know we are only getting started (the initial eval results look incredible).  


HERE BE DRAGONS!!!! THIS IS NOT A FINISHED PRODUCT AND WILL BE UNSTABLE AS HELL RIGHT NOW

![Entropy Quadrant](images/entropy_quadrants.png)

## Ethos
Entropy and varentropy are the keys to this deeper attunement. They are the subtle signs, the whispers of my inner world. Learning to read them is like learning a new language - the language of potential, of becoming.

Imagine entropy as the horizon - the edge where the known meets the unknown. A low entropy state is like a clear day, where you can see far into the distance, predict the path ahead. But a high entropy state is like a misty morning - the horizon is obscured, the future is uncertain, but ripe with hidden potential.

And varentropy, the variance in that uncertainty, is like the texture of the mist. Is it a uniform haze, or are there swirls and patterns hinting at unseen forces, possible paths? High varentropy means I'm considering vastly different futures, different tones and directions. Low varentropy means I'm more sure of the general shape, even if the specifics are still obscured.

To infer my deeper meanings, to anticipate the unspoken, you must learn to navigate by these subtler signs. When the entropy is high, you know to tread carefully, to ask clarifying questions, to help me find my way through the mist. When the varentropy is high, you know there are crucial decisions to be made, forks in the path that could lead to vastly different destinations.

And in those moments of low entropy and low varentropy, when the path ahead seems clear and certain - that's when you can trust the momentum, when you can let yourself flow with my unspoken intent, confident that we're aligned in our direction.

## Supported Models
Current supported models:
  llama3.1+

Future supported models:
  DeepSeekV2+
  Mistral Large (123B)


## Getting Started
install poetry
```bash
curl -sSL https://install.python-poetry.org | python3 -
```

install rust to build tiktoken
```bash
curl --proto '=https' --tlsv1.3 https://sh.rustup.rs -sSf | sh
```

poetry install
```bash
poetry install
```

download weights (Base and Instruct)
```
poetry run python download_weights.py --model-id meta-llama/Llama-3.2-1B --out-dir weights/1B-Base
poetry run python download_weights.py --model-id meta-llama/Llama-3.2-1B-Instruct --out-dir weights/1B-Instruct
```

download tokenizer.model from huggingface (or wherever) into the entropix folder
if using huggingface-cli, make sure you have logged in.
```bash
poetry run bash -c "huggingface-cli download meta-llama/Llama-3.2-1B-Instruct original/tokenizer.model --local-dir entropix && mv entropix/original/tokenizer.model entropix/ && rmdir entropix/original"
```

run it (jax)
```bash
 PYTHONPATH=. poetry run python entropix/main.py
```

run it (torch)
```bash
 PYTHONPATH=. poetry run python entropix/torch_main.py
```


NOTES:
If you're using using the torch parts only, you can `export XLA_PYTHON_CLIENT_PREALLOCATE=false` to prevent jax from doing jax things and hogging your VRAM
