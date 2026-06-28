## 学習項目

- DS pandas, numpy, Seabornを活用できる力を養う

## 初めのコンテナ動かす方法

```
docker run -it \
  -p 8890:8890 \
  --platform linux/amd64 \
  --name python_statistics \
  -v "$(pwd):/work" \
  datascientistus/ds-python-env \
  jupyter lab --ip=0.0.0.0 --allow-root --port=8890 \
  --NotebookApp.token='' \
  --notebook-dir=/work
```

2回目以降

```
docker start -i python_statics
```
# python-data-analysis
- 統計学２級レベル
