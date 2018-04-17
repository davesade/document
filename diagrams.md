## Flowcharts etc.

Native Docsify cannot render diagrams by hand. You could add some pictures, but that should be used only when no other options is available. Similar to [graphs](graphs.md), we can inject some special formatted characters to call plugin for diagrams and flowcharts.  
Docsify does support so called [Mermaid](https://mermaidjs.github.io/), so as long you configure this plugin via `index.html` file, you can *describe* your chart like this:  

```
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

Which will produce following output:  

<div class="mermaid">
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
</div>

Or you can add more complex flow charts like this:

```
sequenceDiagram
    Alice ->> Bob: Hello Bob, how are you?
    Bob-->>John: How about you John?
    Bob--x Alice: I am good thanks!
    Bob-x John: I am good thanks!
    Note right of John: Bob thinks a long<br/>long time, so long<br/>that the text does<br/>not fit on a row.

    Bob-->Alice: Checking with John...
    Alice->John: Yes... John, how are you?
```

Resulting following sequence diagram:  

<div class="mermaid">
sequenceDiagram
    Alice ->> Bob: Hello Bob, how are you?
    Bob-->>John: How about you John?
    Bob--x Alice: I am good thanks!
    Bob-x John: I am good thanks!
    Note right of John: Bob thinks a long<br/>long time, so long<br/>that the text does<br/>not fit on a row.

    Bob-->Alice: Checking with John...
    Alice->John: Yes... John, how are you?
</div>

And why stop here? Mermaid can also do Gantt diagrams. Again, the source code:  
```
gantt
    title A Gantt Diagram
    dateFormat  YYYY-MM-DD
    section Section
    A task           :a1, 2014-01-01, 30d
    Another task     :after a1  , 20d
    section Another
    Task in sec      :2014-01-12  , 12d
    another task      : 24d
```

And the result:  

<div class="mermaid">
gantt
    title A Gantt Diagram
    dateFormat  YYYY-MM-DD
    section Section
    A task           :a1, 2014-01-01, 30d
    Another task     :after a1  , 20d
    section Another
    Task in sec      :2014-01-12  , 12d
    another task      : 24d
</div>

... and ALL of that is actually a source code. However, we left convenient waters of simple MarkDown syntax, so consider this as advanced fancy stuff :).  
And again, checkout the file *diagrams.md* to see real text content of the file you just see with your browser.  
