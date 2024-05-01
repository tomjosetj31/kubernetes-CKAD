# Node Selectors

## Label Nodes

```bash
kubectl label nodes <node-name> <label-key>=<label-value>
```

example: `kubectl label nodes node-1 size=large`

## Drawback

can't use advanced queries like or, and, in, not, etc.
