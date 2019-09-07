# Simple Fusion Visualization
This tool visualize a fused list and component lists simply using d3.js

see the following demos.

- [Simple demo](https://sosuke-k.github.io/simple-fusion-visualization/index.html?data=data1.json).
- [Legend demo](https://sosuke-k.github.io/simple-fusion-visualization/index.html?data=data2.json).

## How to use

### Prepare data

- You have to prepare a json file like [this](./data1.json).

```
{
  "name": "F",
  "documents": [
    { "doc_id": "1", "score": "202.0", "color": "#E8411C"},
    { "doc_id": "3", "score": "138.0", "color": "#B0B0B0"},
    { "doc_id": "4", "score": "67.0", "color": "#730A0B"}
  ],
  "children": [
    {
      "name": "S1",
      "documents": [
        { "doc_id": "1", "score": "63.0", "color": "#E8411C"},
        { "doc_id": "2", "score": "40.0", "color": "#B0B0B0"},
        { "doc_id": "3", "score": "39.0", "color": "#B0B0B0"}
      ]
    },
    {
      "name": "S2",
      "documents": [
        { "doc_id": "4", "score": "67.0", "color": "#730A0B"},
        { "doc_id": "1", "score": "38.0", "color": "#E8411C"},
        { "doc_id": "3", "score": "30.0", "color": "#B0B0B0"}
      ]
    }
  ]
}
```

### Clone and Run

```
git clone https://github.com/sosuke-k/simple-fusion-visualization
cd simple-fusion-visualization
python -m http.server 8000 # you don't have to use python
```

then, open http://localhost:8000/index.html?data= &lt;path to json file&gt; .
