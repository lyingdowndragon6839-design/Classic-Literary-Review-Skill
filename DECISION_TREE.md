# Decision Tree

Use this file when the user request is unclear, incomplete, or not a standard “write a full reading response” task.

## Main Routing

```mermaid
flowchart TD
    A["User asks for reading response"] --> B{"Has the user finished the book?"}
    B -- "No" --> C["Build reading frame; do not fake completion"]
    B -- "Yes" --> D{"Does the user have feelings or notes?"}
    D -- "No / very little" --> E["Search and offer angles first"]
    D -- "Yes" --> F["Preserve user's feeling as primary clue"]
    F --> G{"Does the user have a draft?"}
    E --> H["Generate candidate main judgments"]
    G -- "Yes" --> I["Revision-first workflow"]
    G -- "No" --> H
    H --> J{"Target scene?"}
    J -- "Classroom" --> K["Clear structure, moderate voice"]
    J -- "Zhihu" --> L["Sharper opening, argument-forward"]
    J -- "Douban" --> M["Personal reading texture"]
    J -- "Public account" --> N["Polished essay rhythm"]
    K --> O["Outline -> Draft -> Review -> AI Check"]
    L --> O
    M --> O
    N --> O
    I --> P["Preserve intent -> repair logic -> reduce AI trace"]
    P --> O
```

## Common Cases

### User Has Not Finished The Book

Do:

- build a character and conflict map;
- list questions to watch while reading;
- suggest possible angles after finishing.

Do not:

- write “读完整本书后我觉得”;
- invent personal reading reactions.

### User Has Only One Feeling

One feeling is enough. Treat it as a seed.

```text
我最难受的是福贵最后只剩老牛。
```

Turn it into:

```text
Main judgment: 《活着》不是把苦难写成伟大，而是写人被磨空以后仍然还在活着。
```

### User Already Has A Draft

Start with editing, not rewriting.

| Step | Action |
|---|---|
| 1 | Identify the user's main intent |
| 2 | Mark AI cliches and empty claims |
| 3 | Repair logic and evidence |
| 4 | Preserve voice |
| 5 | Produce a revised version |

### User Wants “降 AI”

Look beyond phrases:

- sentence rhythm;
- paragraph shape;
- plot-to-judgment connection;
- generic ending;
- missing reading process.

### User Needs Classroom Submission

Keep it clear. Do not over-style.

Good classroom reading responses usually have:

- one main judgment;
- a few concrete details;
- moderate personal voice;
- no internet slang;
- no empty moral ending.

