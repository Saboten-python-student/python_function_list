# pygrib 関数・メソッド一覧

## 🔹 基本構成
| 名前 | 概要 |
|------|------|
| `pygrib.open()` | GRIBファイルを開く（イテレータ取得） |
| `grb.select()` | メッセージの条件抽出（変数、時間、高度など） |
| `grb.message(index)` | 指定番号のメッセージを取得 |
| `grb.read()` | 全メッセージをリストとして取得 |

## 🔹 GRIBメッセージの属性（1つの変数データ）
| 属性名 | 概要 |
|--------|------|
| `grb.name` | 変数名（例：Temperature） |
| `grb.shortName` | 省略名（例：t） |
| `grb.level` | 高度（例：850） |
| `grb.validDate` | 有効日時 |
| `grb.units` | 単位（例：K, m/s） |
| `grb.values` | データ本体（2次元配列） |
| `grb.latlons()` | 緯度・経度の2次元配列を取得 |

## 🔹 代表的な処理フロー
```python
import pygrib
grbs = pygrib.open("sample.grib2")

# 指定条件でメッセージ取得
t850 = grbs.select(name="Temperature", level=850)[0]

# 値と座標の取得
data = t850.values
lats, lons = t850.latlons()
```

## 🔹 注意点
- `pygrib` の内部は **eccodes** に依存しており、事前にCライブラリが必要です
- ファイルが大きい場合は `.read()` より `for grb in grbs:` が推奨されます
