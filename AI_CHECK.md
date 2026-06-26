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

