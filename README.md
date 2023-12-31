# imagenet_labels

```python
def get_imagenet_labels():
    import json
    with open('./imagenet_labels.json', 'r') as file:
        json_data = json.load(file)
    labels = {int(idx):label for idx, label in json_data.items()}
    return labels

IMAGENET_LABELS = get_imagenet_labels()
```