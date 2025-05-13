# Plotly 関数・モジュール一覧（Python版）

## 🔹 基本構成
| 名前 | 概要 |
|------|------|
| `plotly.graph_objects`（`go`） | グラフオブジェクトを直接定義（柔軟・詳細） |
| `plotly.express`（`px`） | 高レベルAPIで簡単に可視化（短く書ける） |

## 🔹 主要な図表（Express版）
| 名前 | 概要 |
|------|------|
| `px.line()` | 折れ線グラフ |
| `px.scatter()` | 散布図 |
| `px.bar()` | 棒グラフ |
| `px.density_contour()` | 密度等高線図 |
| `px.imshow()` | 画像／2Dカラーマップ表示 |
| `px.line_3d()`, `px.scatter_3d()` | 3D折れ線・散布図 |

## 🔹 グラフオブジェクト（go）による柔軟な構成
| 名前 | 概要 |
|------|------|
| `go.Figure()` | 図全体のオブジェクト |
| `go.Scatter()`, `go.Bar()`, `go.Surface()` | 各種トレース（描画要素） |
| `fig.add_trace()` | トレースの追加 |
| `fig.update_layout()` | 全体のレイアウト設定 |
| `fig.update_traces()` | トレース共通設定の一括更新 |
| `fig.show()` | 描画表示 |

## 🔹 インタラクティブ制御
| 名前 | 概要 |
|------|------|
| `fig.update_xaxes()`, `update_yaxes()` | 軸の設定 |
| `fig.add_annotation()` | 注釈・矢印の追加 |
| `fig.add_shape()` | 線・長方形などの図形追加 |
| `fig.update_layout(sliders=...)` | スライダーによる可変プロット |
| `plotly.subplots.make_subplots()` | サブプロットの作成 |

## 🔹 保存・エクスポート
| 名前 | 概要 |
|------|------|
| `fig.write_image()` | PNGやSVGへの出力（kaleidoが必要） |
| `fig.write_html()` | HTMLファイルに出力 |
