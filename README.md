# 🔍 GemLens GitHub Action

Run **GemLens** automatically in GitHub Actions to analyze how your `Gemfile`
evolved over time.

## 🚀 Usage

Add this workflow to your repository:

```yaml
name: GemLens

on:
  pull_request:
  push:
    branches: [main]

jobs:
  gemlens:
    runs-on: ubuntu-latest
    steps:
      - uses: BestBitsLab/gemlens-action@v1
```

## 📦 What it does

- Detects added, removed, and updated gems
- Prints a readable timeline
- Works with any Git-tracked Ruby project

Powered by the gemlens Ruby gem.
[gemlens](https://github.com/BestBitsLab/gemlens)
