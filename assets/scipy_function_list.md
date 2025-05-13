# SciPy 関数・モジュール一覧

## 🔹 基本構成（主要モジュール）
| モジュール | 概要 |
|------------|------|
| `scipy.integrate` | 数値積分（常微分方程式の解法など） |
| `scipy.optimize` | 最適化・方程式の数値解法 |
| `scipy.interpolate` | 補間（線形・スプラインなど） |
| `scipy.fft` | 高速フーリエ変換（FFT） |
| `scipy.linalg` | 線形代数（NumPyの上位互換） |
| `scipy.signal` | 信号処理（フィルタ、畳み込みなど） |
| `scipy.stats` | 統計処理・確率分布 |
| `scipy.spatial` | 空間解析（距離、KD-tree） |

## 🔹 integrate（積分・微分方程式）
| 名前 | 概要 |
|------|------|
| `quad()` | 一変数の数値積分 |
| `dblquad()` | 二重積分 |
| `solve_ivp()` | 常微分方程式（IVP）の数値解 |
| `odeint()` | ODEの数値積分（古典的） |

## 🔹 optimize（最適化）
| 名前 | 概要 |
|------|------|
| `minimize()` | 最小化（多目的関数） |
| `root()` | 方程式の数値解法 |
| `curve_fit()` | 曲線フィッティング（回帰） |
| `least_squares()` | 最小二乗法 |

## 🔹 interpolate（補間）
| 名前 | 概要 |
|------|------|
| `interp1d()` | 1次元補間（線形・スプライン） |
| `interp2d()` | 2次元補間（旧式・非推奨） |
| `griddata()` | 任意点の格子補間 |
| `UnivariateSpline` | スプライン補間クラス |

## 🔹 fft（高速フーリエ変換）
| 名前 | 概要 |
|------|------|
| `fft()`, `ifft()` | フーリエ変換／逆変換 |
| `rfft()`, `irfft()` | 実数高速変換 |
| `fftfreq()` | 周波数の計算 |

## 🔹 linalg（線形代数）
| 名前 | 概要 |
|------|------|
| `inv()`, `det()` | 逆行列、行列式 |
| `solve()`, `eig()` | 連立方程式、固有値問題 |
| `svd()` | 特異値分解 |

## 🔹 stats（統計・確率分布）
| 名前 | 概要 |
|------|------|
| `norm`, `binom`, `poisson` | 各種確率分布オブジェクト |
| `pdf()`, `cdf()`, `ppf()` | 確率密度・累積分布・分位点 |
| `mean()`, `std()`, `var()` | 各種統計量 |
| `ttest_ind()`, `pearsonr()` | t検定、相関係数 |

