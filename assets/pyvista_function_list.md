# PyVista 関数・メソッド一覧

## 🔹 基本構成
| 名前 | 概要 |
|------|------|
| `pv.Plotter()` | 3D描画用のプロッタ作成 |
| `pv.read()` | VTKファイルなどの読み込み |
| `pv.wrap()` | NumPy配列などをPyVistaオブジェクトに変換 |
| `pv.UniformGrid()` | 等間隔の格子データ作成 |

## 🔹 メッシュ作成・操作
| 名前 | 概要 |
|------|------|
| `add_mesh()` | 表示対象のメッシュ・ボリュームを追加 |
| `threshold()` | 指定範囲での抽出（等値面マスク） |
| `slice()`, `slice_orthogonal()` | スライス（断面）表示 |
| `contour()` | 等値面の抽出 |
| `clip()` | 指定平面での切断表示 |
| `decimate()` | ポリゴン数を減らす簡略化処理 |

## 🔹 描画設定
| 名前 | 概要 |
|------|------|
| `show()` | 描画ウィンドウの表示 |
| `add_scalar_bar()` | カラーバーの追加 |
| `add_axes()` | 座標軸の追加 |
| `camera_position` | 視点位置の設定 |
| `update()` | 描画更新（アニメーションなどで使用） |

## 🔹 配色・スタイル
| 名前 | 概要 |
|------|------|
| `cmap=` | カラーマップ（例：`cmap="coolwarm"`） |
| `opacity=` | 不透明度の指定（0〜1またはリスト） |
| `show_edges=True` | メッシュのエッジを表示 |
| `smooth_shading=True` | 表面を滑らかに表示 |

## 🔹 補助機能・出力
| 名前 | 概要 |
|------|------|
| `export_html()` | Web表示用に出力 |
| `screenshot()` | 画像として保存 |
| `plot_off_screen=True` | GUIを使わず描画（サーバー用など） |

