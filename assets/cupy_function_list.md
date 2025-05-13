# CuPy 関数・メソッド一覧

## 🔹 配列の作成
| 名前 | 概要 |
|------|------|
| `cupy.array()` | PythonリストやNumPy配列からCuPy配列を作成 |
| `cupy.zeros()`, `cupy.ones()`, `cupy.empty()` | 初期化済み配列の生成 |
| `cupy.arange()`, `cupy.linspace()` | 等間隔の配列生成 |
| `cupy.full()` | 任意の値で埋める配列生成 |

## 🔹 基本演算（NumPyと同様のAPI）
| 名前 | 概要 |
|------|------|
| `cupy.add()`, `cupy.subtract()` | 加減算 |
| `cupy.multiply()`, `cupy.divide()` | 乗除算 |
| `cupy.power()`, `cupy.mod()` | 累乗、剰余 |
| `cupy.exp()`, `cupy.log()`, `cupy.sqrt()` | 指数・対数・平方根 |

## 🔹 配列操作
| 名前 | 概要 |
|------|------|
| `cupy.reshape()`, `cupy.transpose()` | 形状変更・軸の入れ替え |
| `cupy.concatenate()`, `cupy.stack()` | 配列の結合 |
| `cupy.ravel()`, `cupy.flatten()` | 一次元化 |
| `cupy.copy()` | 配列のコピー |

## 🔹 統計・集約処理
| 名前 | 概要 |
|------|------|
| `cupy.mean()`, `cupy.std()`, `cupy.var()` | 平均、標準偏差、分散 |
| `cupy.min()`, `cupy.max()` | 最小・最大値 |
| `cupy.sum()`, `cupy.prod()` | 総和、積 |

## 🔹 条件・論理演算
| 名前 | 概要 |
|------|------|
| `cupy.where()` | 条件に応じた値の選択 |
| `cupy.isnan()`, `cupy.isfinite()` | NaN、有限値の検出 |
| `cupy.any()`, `cupy.all()` | 論理積・和の集約 |

## 🔹 高速演算・特殊処理
| 名前 | 概要 |
|------|------|
| `cupy.fft.fft()`, `ifft()` | 高速フーリエ変換（FFT） |
| `cupy.linalg.inv()`, `svd()`, `solve()` | 線形代数（行列計算） |
| `cupy.asnumpy()` | CuPy配列をNumPy配列に変換 |
| `cupy.cuda.Device()` | CUDAデバイスの制御 |
