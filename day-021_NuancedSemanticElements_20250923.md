# Day 21: Lecture - Understanding Nuanced Semantic Elements

Chit-chat: I'm nog going to complain about sleeplessness from now on. Becasue this is the new norm now 😅

## Key topics covered: 
(I haven't been using the .md template I created as I ended up mostly creating from scratch anyway so had forgotten about this which I think is still good to keep)
- [x] emphasis `em` element vs. idiomatic `i` element
- [x] strong `strong` element vs. bring attention to element (which one is this - `bold`?)
- [x] description lists (this is new)

## 1. When to use emphasis `em` element vs. idiomatic `i` element
### 1.1 `i`
**Presentational** element that shows that it's somehow different from the surrounding text (e.g., highlighting alternative voice or mood, idiomatic terms from another language, technical terms, and thoughts)

Example:

```
<p>There is a certain <i lang="fr">je ne sais quoi</i> in the air.</p>
```
### 1.2 `em`
**Semantic** element to represent a special emphasis to <em>only</em> a few words compared to surrounding text

<br></br>
<ins>It's important to know that these elements should not be used for presentational purposes only. If you need to display the text in italics, but the text doesn't have a special purpose, style, or meaning in the paragraph, you should use CSS instead.</ins>   
> Don't quite understand what this <i>actually</i> means

[Ends 09:15]

---


## 2. When to use strong `strong` element vs. bring attention to element
Visually similar (text is bold), but quite different in meanings.
### 2.1 "bring attention to" element i.e. `b` 
Only draws attention to the text, without indicating the higher level of importance/urgency - **Q**: does this make it "presentational" element?
> Example: use in summaries or product reviews
```
<p>
We tested several products, including the <b>SuperSound 3000</b> for audio quality, the <b>QuickCharge Pro</b> for fast charging,
and the <b>EcoClean Vacuum</b> for cleaning. The first two performed well, but the <b>EcoClean Vacuum</b> did not meet expectations.
</p>
```

### 2.2 `strong` element
A **semantic** HTML element that emphasizes text that is crucial, or urgent.
> Example: allergy information
```
<p>
<strong>Warning:</strong> This product may cause allergic reactions.
</p>
```

**Q**: now a bit confused between `b`, `strong` and `em`, `i`.

## 3. What are and when to use description lists
Essentially, when you have two related pieces of information in a **key-value** pair format, where one acts as a label (the key), and the other acts as additional related information (the value), you can use a description list.
- `dl` description list
- `dt` description term
- `dd` description details
Example: product specifications, frequently asked questions, contact information, and metadata.
```
<dl>
  <dt>Flour</dt>
  <dd>2 cups</dd>
  <dt>Sugar</dt>
  <dd>1/2 cup</dd>
</dl>
```
Render:

<img width="258" height="174" alt="image" src="https://github.com/user-attachments/assets/46b3f0a0-8159-41b9-b321-dab0e41fc61d" />

[Ends 20:12]

## What went well
N/A

## What didn't go well
1. Feels like the entire course lacks the real-time typein-result rendering pair, though do appreciate the "lecture" format rather than video as I follow better and find it more efficient when it comes to self-pace
2. In a way, too much "lecture" with not very beginner-friendly content structure, and no comparison with potential confusion e.g. dl versus ul or ol, or how do we make it more visually appealing as currently the dt and dd alignment/indentation makes it look bad (maybe this will be covered later in this lecture)
