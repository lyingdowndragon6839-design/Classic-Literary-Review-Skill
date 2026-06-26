# AI Trace Detection Module

## Rule

When AI trace is detected, rewrite directly. Do not merely warn.

## Phrase Detection

Automatically rewrite paragraphs containing:

| Pattern | Problem | Rewrite Direction |
|---|---|---|
| 体现了 | Empty explanation verb | Name the detail and its effect |
| 揭示了 | Overclaim | State what the scene lets us see |
| 反映了 | Vague social link | Identify the concrete social mechanism |
| 由此可见 | School essay transition | Move directly to judgment |
| 值得我们思考 | Generic ending | Ask a specific unresolved question |
| 具有重要意义 | Empty value claim | State who changes, and how |
| 引人深思 | Placeholder emotion | Describe the discomfort |
| 发人深省 | Cliche | Replace with a scene or choice |
| 深化主题 | Textbook phrase | Explain how the thesis changes |
| 升华主题 | Textbook phrase | Return to final image |
| 命运的无常 | Abstract fatalism | Show the sequence of losses |
| 人性的光辉 | Empty praise | Name the cost of the action |

## Rhythm Detection

Check:

- Are paragraphs nearly equal length?
- Are sentences mostly the same length?
- Are there too many parallel clauses?
- Does every paragraph end with summary?
- Does the article repeatedly use “这说明” or “这让我们看到”?
- Does the ending sound like moral education?

## 读后感高频 AI 腔

检测到下面表达时，直接改写，不要只是提醒。

| 错误表达 | 替代表达 |
|---|---|
| 这本书让我受益匪浅 | 我合上书以后，最先想到的不是“收获”，而是一种说不清的沉重。 |
| 引人深思 | 这一幕真正留住人的，是它没有把问题说完。 |
| 发人深省 | 读到这里，人很难再轻易下判断。 |
| 体现了人性的光辉 | 这个选择之所以动人，是因为他明明可以少承担一点，却还是没有退开。 |
| 揭示了社会的黑暗 | 小说让人看见，黑暗不是抽象背景，而是工资、身份、名声和机会一点点压到人身上。 |
| 反映了时代的悲剧 | 悲剧不是时代两个字造成的，而是那个时代让人只剩下很窄的选择。 |
| 命运的无常 | 生活刚给他一点落脚处，下一页就把那点落脚处撤走。 |
| 苦难中的希望 | 希望在这里并不明亮，它只是人在撑不下去时还没松手。 |
| 生命的意义 | 这本书没有急着回答意义，它只是逼人看见一个人为什么还继续活着。 |
| 让我明白了 | 我读到最后才意识到，原来前面那些细节一直在把人推向这个结局。 |
| 值得我们每个人思考 | 这个问题并不宏大，却很难躲开：换成我们，会不会也做出相似选择？ |
| 总而言之 | 到这里，不需要再总结；那个场景本身已经把话说完了。 |
| 由此可见 | 也正因为这个细节，前面对人物的判断才突然变得不那么简单。 |
| 深化了主题 | 它让文章的问题从“发生了什么”变成“人为什么只能这样选择”。 |
| 升华了主旨 | 结尾没有把主题抬高，而是把读者重新按回那个具体的人身上。 |

## Automatic Repair Patterns

### From Explanation To Observation

Bad:

```text
这一情节体现了人物内心的复杂。
```

Rewrite:

```text
真正复杂的不是他犹豫，而是他已经知道该怎么做，却仍然把手停在门边，好像再多站一秒，责任就会自动离开。
```

### From Abstract To Concrete

Bad:

```text
作品揭示了命运的无常。
```

Rewrite:

```text
作品没有急着谈命运。它只是让一个人刚刚以为生活有了落脚处，下一页就把那点落脚处撤掉。
```

### From Summary To Open Wound

Bad:

```text
总而言之，这本书给我们深刻启示。
```

Rewrite:

```text
读完以后，最难放下的不是结局，而是人物在结局前那几次本可以说真话却没有说的停顿。
```

## AI Check Report

Report:

| Check | Result | Fix Applied |
|---|---|---|
| Cliche phrases |  |  |
| Paragraph length |  |  |
| Sentence rhythm |  |  |
| Empty praise |  |  |
| Plot overuse |  |  |
| Repeated transitions |  |  |
| Final moralizing |  |  |
