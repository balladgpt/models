# BalladGPT Models

Unfortunately, due to the high cost of hosting LFS on GitHub, we've moved the models to HuggingFace. You can download the models [here](https://huggingface.co/balladgpt/balladgpt-v2).

# Model Card

This is the latest version BalladGPT. [You can try the old BalladGPT here](https://huggingface.co/balladgpt/balladgpt-old-v1). The old BalladGPT's dataset size was 568 KB, whereas the NEW BalladGPT's dataset size is 926 KB.

## Usage

**Note:** BalladGPT's dataset is relatively small, so the quality is not optimal. If possible, please consider using a newer generation of GPT as these will equal or surpass this model in quality and speed. **Please see the example results at the bottom of the page to evaluate this model's quality.**

You can use BalladGPT as you would use any other GPT-2-based model:

```python
from transformers import pipeline
generator = pipeline('text-generation', model='balladgpt/balladgpt-v2')
print(generator("Once upon a time", do_sample=True, min_length=20)[0]['generated_text'])
```

You can also use CUDA or MPS if available.

```python
generator.to('cuda') # Pipe to CUDA
generator.to('mps') # Pipe to MPS
```

## Biases

As this model was trained on select literature from the 18th, 19th, 20th century, certain biases and sterotypes may be expressed in generated texts which are neither endorsed or supported by the author of this model and are purely results of the literature used to train this model.

## Disclaimer

The author of this model takes no responsibility for any content generated or any misuse of the model.

## Training Data

BalladGPT was trained on various ballads and poems in the public domain.

BalladGPT is a fine-tuned version of GPT-2.

The BalladGPT dataset is not available at the present moment.

## Training Information

- Dataset Size: 926 KB
- Date Trained: March 18, 2023

## Updates

We are not intending to update this model.

## Example Results

These are example results with no prompts. Some of these examples may express sterotypes and biases which are a result of the training data. These sterotypes and biases are not supported or endorsed by the creator of this model and are purely results of the literature used in training data. Due to the cost and difficulty of removing all biases and sterotypes, some have been left in the training data. Please use this model with caution.

```
And how you were once again
A good-faith prophet in the West?
I saw you on my journey!
Were you in the country and the hills
From which we came,
To bring them good food and good wine
```

```
-The King of England
Who came to Scotland,
And made Scotland proud
And settled it within his rule
Of merry men.
-He brought us up as fair-minded men,
And brought us up to England.
```

```
To my wife's house the bride-maid is,
For the groom's wife, and his wife a bride.
Then he gave that good man's bride-maid's name-
I know not what is it,
```

```
That we are at war:
There is no man of mine who fears or knows
He is at peace at last:
I want the strength of God's wrath to be strong
Until then, before we shall die,
```

```
'I think the good of this world is not too high,' said Lord Arthur.
'In thy world,' said the Earl of Edinburgh.
It was the happiest life that ever lived!
And the sweet sound which our world's loud
```

```
The other way home,
Before the good home of Adam,
Beneath the black and the gray.
The other way home, before the great sun of heaven,
Beneath the black and the gray.
```

```
Where he has lived his life in the fields, where he lives in a place that grows in summer;
Where he has died with some fresh flower,
In a night of flower and snow,
The world is full of stars,
```

```
There's no word as they play:
They sang that they were no sooner to make.
From what hear they hear,
With what eye they eye,
Shouting for their songs that sound,
The joy that they have
```

```
Ye'lt ye found there,
Ye were alone there,
And the only one in whom you
Had known the story
I must have told,
And have seen the great thing of your heart.
Oh, what love
```

```
'God that art,' says the Prince of Rome,
This may be our faith of God;
Welcoming of our Mother!'
The Pope's letter to me is the gift he gave me,
From the old-fashioned hand
```

```
'Til I leave you, if I will not,
This shall be a place and a place no more!'
His eyes flashed across the black
He called his name:
He was God's soul mate,' he said.
```

```
Her face,
Shining in all the dark
Of a soul without a soul,
To speak of her faith's light.
So when I read her own tears at a glance
Singing of hope in old age,
```

```
He that hath a sword and a sword-sword,
And when the war is upon, the king's sons who serve
The country's glory
The war without, and his armies that war
```

```
The best in their midst?
I will not lose my good old man
With the way of love!"
"You were my dear mother, and for all your love
I had a way of saying,
```

```
The mason's work was done,
And the farmer's came to him
And asked him:
"Where are we on the road, now?"
And that he answered, "Out of the forest and forest-land?"
```

```
The rich and free, and the poor, all together,
And the rich on the bankowed road,
And the poor on the bankowed road, with torches in tow,
All looking for light, all looking for warmth!
```

```
I shall go to London for the night.
A merry morning will come near my door,
But after a sweet evening in town,
I'll return my fair and cheerful heart.
And I'll pass, all in my fancy's
```

```
The Sun's dark
Shalt not rise to be light'd
There-tooth's long-dead tree,
Shalt be darkness.
For the hour, after hour,
Stretching to the moon,
```

```
In the morning air that you breath,
Til water rose and the heat faded, your eyes came to the stars of day;
O'er the trees and green fields and fresh snow-bough
Of summer's day
```

```
Her heart aching again;
And in her hand the young boy cried:
"Have you no gold? have you no jewels,
Or gold-digger's guide's guide
```

```
It is a story of some
This was his journey,
That, with some lightness, he fell,
The journey of life was not at hand
Upon a road to heaven;
For he heard it with sorrow, with love
```

```
He held me to the door,
I was there to be;
Than I walked the path
Of youth in springy-green and rosewood-tree;
"What's the charm of summer?"
The birds that sing
```
