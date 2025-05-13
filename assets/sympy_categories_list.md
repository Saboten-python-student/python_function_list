
# SymPy 関数・クラス一覧（カテゴリ別）

## 🔹 1. sympy.core – 基本構成要素（式・数値・記号）
| 名前 | 概要 |
|------|------|
| `Symbol` | 記号（変数） |
| `symbols` | 複数記号の生成 |
| `Integer`, `Rational`, `Float` | 数値型（有理数、実数） |
| `Eq`, `Ne`, `Lt`, `Gt` | 等号・不等号 |
| `Add`, `Mul`, `Pow` | 四則演算オブジェクト |
| `S` | 定数生成用オブジェクト (`S(1)/2`など) |

## 🔹 2. sympy.simplify – 式の簡単化・整理
| 名前 | 概要 |
|------|------|
| `simplify` | 自動簡単化（万能だが重い） |
| `expand`, `factor`, `cancel`, `collect` | 括弧展開・因数分解・通分・項まとめ |
| `trigsimp`, `powsimp`, `logcombine` | 三角関数・べき・対数の整理 |
| `nsimplify` | 数値の近似的な簡略表現（πなど） |

## 🔹 3. sympy.functions – 数学関数
| 名前 | 概要 |
|------|------|
| `sin`, `cos`, `tan`, `exp`, `log`, `sqrt`, `Abs` | 一般的な関数 |
| `asin`, `acos`, `atan`, `sinh`, `cosh`, `atanh` | 逆三角関数・双曲線関数 |
| `gamma`, `zeta`, `factorial`, `loggamma` | 特殊関数 |

## 🔹 4. sympy.calculus – 微分・積分・極限
| 名前 | 概要 |
|------|------|
| `diff` | 微分 |
| `integrate` | 積分 |
| `limit` | 極限値 |
| `series` | 級数展開（テイラー展開） |
| `singularities` | 特異点の計算 |

## 🔹 5. sympy.solvers – 方程式の解法
| 名前 | 概要 |
|------|------|
| `solve` | 一般的な方程式解法 |
| `solveset`, `linsolve`, `nonlinsolve` | より厳密な集合解法 |
| `dsolve` | 常微分方程式の解法 |
| `checksol` | 解が正しいかの検証 |

## 🔹 6. sympy.matrices – 行列・線形代数
| 名前 | 概要 |
|------|------|
| `Matrix` | 行列オブジェクト |
| `eye`, `zeros`, `ones` | 単位行列、ゼロ、1行列 |
| `.det()`, `.inv()`, `.T` | 行列式、逆行列、転置 |
| `.rref()` | 行基本形（簡約化） |
| `.eigenvals()`, `.eigenvects()` | 固有値・固有ベクトル |

## 🔹 7. sympy.logic – 論理演算・集合
| 名前 | 概要 |
|------|------|
| `And`, `Or`, `Not`, `Implies` | 論理演算子 |
| `true`, `false` | 真理値 |
| `BooleanFunction` | ブール関数の親クラス |
| `satisfiable` | 論理式の充足可能性判定 |

## 🔹 8. sympy.sets – 集合と区間
| 名前 | 概要 |
|------|------|
| `Interval`, `Union`, `Intersection` | 区間・集合演算 |
| `EmptySet`, `FiniteSet`, `Naturals`, `Reals` | 代表的集合 |
| `Contains` | 所属判定 |

## 🔹 9. sympy.stats – 確率・統計
| 名前 | 概要 |
|------|------|
| `Normal`, `Uniform`, `Die` | 確率変数（正規分布など） |
| `E`, `P`, `density`, `cdf` | 期待値、確率、密度、累積分布 |
| `sample`, `variance`, `std` | サンプリング、分散、標準偏差 |

## 🔹 10. sympy.geometry – 幾何学
| 名前 | 概要 |
|------|------|
| `Point`, `Line`, `Segment`, `Circle` | 基本図形 |
| `intersection`, `are_similar` | 幾何演算・関係 |

## 🔹 11. sympy.plotting – グラフ描画
| 名前 | 概要 |
|------|------|
| `plot`, `plot3d`, `plot_implicit` | 2D/3D描画 |
| `Plot` オブジェクト | 複数グラフの統合管理 |

## 🔹 12. sympy.utilities – 補助ツール
| 名前 | 概要 |
|------|------|
| `lambdify` | 式をPython関数化（高速処理に） |
| `pycode`, `ccode`, `latex` | 他言語コードやLaTeX変換 |
| `numbered_symbols` | 連番付き記号生成 |
