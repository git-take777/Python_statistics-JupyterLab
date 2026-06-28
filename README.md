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

- 記述統計と推測統計
    - 母集団からランダムに取り出し、標本から母集団の特徴を推測する。
    - 標本: 母集団からランダムなデータを抽出
    - 統計といったら推測統計を指すところが多い。
    - 統計学を学ぶ人のGoalは最終的に目指しているのは推測統計から母集団を推測すること
    - 推測統計を学ぶには、記述統計を学ぶ必要がある。
    - 記述統計は標本がどうなっているかを記述する統計学。