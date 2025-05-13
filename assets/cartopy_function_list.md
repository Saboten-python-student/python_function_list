# Cartopy 関数・メソッド一覧

## 🔹 基本構成
| 名前 | 概要 |
|------|------|
| `cartopy.crs` | 座標参照系（投影法）の定義モジュール |
| `cartopy.feature` | 地図上の自然・行政情報の提供モジュール |
| `ccrs` | よく使うCRS（`import cartopy.crs as ccrs`） |
| `cfeature` | よく使うFeature（`import cartopy.feature as cfeature`） |

## 🔹 代表的な座標参照系（CRS）
| 名前 | 概要 |
|------|------|
| `ccrs.PlateCarree()` | 緯度経度そのまま（等間隔） |
| `ccrs.Mercator()` | メルカトル投影 |
| `ccrs.LambertConformal()` | ランベルト正角円錐図法 |
| `ccrs.Orthographic()` | 正射投影（地球を丸く） |

## 🔹 地図要素の追加（Feature）
| 名前 | 概要 |
|------|------|
| `cfeature.COASTLINE` | 海岸線 |
| `cfeature.BORDERS` | 国境線 |
| `cfeature.LAKES` | 湖 |
| `cfeature.RIVERS` | 川 |
| `cfeature.STATES` | アメリカ州境界（国内線） |
| `cfeature.LAND`, `cfeature.OCEAN` | 陸地・海洋 |

## 🔹 Axes（地図）の作成と操作
| 名前 | 概要 |
|------|------|
| `plt.axes(projection=ccrs.X)` | 地図軸の作成 |
| `ax.set_extent([lon_min, lon_max, lat_min, lat_max])` | 表示範囲の設定 |
| `ax.coastlines()` | 海岸線の描画（簡易） |
| `ax.gridlines()` | 緯度経度線の描画 |
| `ax.add_feature()` | 任意の地理要素を追加 |
| `ax.text()`, `ax.plot()` | テキストや点・線の描画（地図上） |

## 🔹 高度な地図表示
| 名前 | 概要 |
|------|------|
| `transform=ccrs.PlateCarree()` | データ座標系の指定（描画時） |
| `ax.contourf(..., transform=ccrs.X)` | 等値図の地図上描画 |
| `ax.pcolormesh(..., transform=ccrs.X)` | カラーマップの描画 |
| `ax.scatter(..., transform=ccrs.X)` | 点群データの表示 |

