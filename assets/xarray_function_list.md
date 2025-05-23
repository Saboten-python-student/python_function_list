# xarray 関数・メソッド一覧

## 🔹 データの読み込みと基本操作
| 名前 | 概要 |
|------|------|
| `open_dataset()` | NetCDFなどからデータセットを読み込む |
| `open_mfdataset()` | 複数ファイルを一括で読み込む |
| `.sel()` | 指定座標の最近傍データを抽出 |
| `.isel()` | インデックス番号でデータを抽出 |
| `.squeeze()` | サイズ1の次元を除去 |
| `.transpose()` | 次元の順番を並び替える |

## 🔹 データ解析・統計処理
| 名前 | 概要 |
|------|------|
| `.mean(dim=)` | 指定次元で平均を取る |
| `.sum(dim=)` | 指定次元で合計を取る |
| `.std(dim=)` | 標準偏差 |
| `.max(dim=)` / `.min(dim=)` | 最大・最小値の取得 |
| `.rolling()` | 移動平均などのロール処理 |
| `.groupby()` | 時間などの属性でグループ化 |

## 🔹 データ構造・変換
| 名前 | 概要 |
|------|------|
| `.values` | NumPy配列として取得 |
| `.to_dataframe()` | pandas DataFrameに変換 |
| `.expand_dims()` | 新しい次元を追加 |
| `.stack()` / `.unstack()` | 次元の合成・分解 |
| `.rename()` | 次元や変数の名前変更 |

## 🔹 補助操作
| 名前 | 概要 |
|------|------|
| `.load()` | データを読み込み（遅延読み込みの解消） |
| `.compute()` | Daskなどの遅延評価を実行 |
| `.plot()` | 簡易的な可視化（matplotlibベース） |
