# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.3.0] - 2026-01-15

### Added
- アコーディオン表示機能を天体イベント情報パネルに実装
- クリックで各パネルを個別に展開/折りたたみ可能
- chevron-downアイコンで展開状態を視覚的に表示（展開時に180度回転）
- ホバー効果を追加してクリック可能であることを明示

### Changed
- 天体イベント情報パネルをグリッドレイアウトから縦積みアコーディオン形式に変更
- デフォルトで全パネルを折りたたみ状態に設定し、縦スペースを大幅に削減

### Removed
- ISS現在位置パネルを削除（Open Notify API の不安定性のため）
- ISS乗員情報パネルを削除（Open Notify API の不安定性のため）
- ISS関連のJavaScript関数（fetchISSLocation, fetchAstronauts）を削除
- READMEからOpen Notify API関連の記述を削除

## [2.2.0] - 2026-01-15

### Added
- ISS現在位置表示機能を追加
- Open Notify API でリアルタイムISS位置情報（緯度・経度・タイムスタンプ）を取得・表示

### Changed
- ISS通過予報をISS現在位置表示に完全移行
- Open Notify API エンドポイントを /iss-pass.json から /iss-now.json に変更

## [2.1.0] - 2026-01-14

### Added
- ISS乗員情報表示機能を追加
- 現在ISSに滞在中の宇宙飛行士の人数と名前をリアルタイム表示
- Open Notify API の /astros.json エンドポイントを統合

## [2.0.0] - 2026-01-14

### Added
- 星空視認性スコア機能（雲量・月明かり・湿度・視程・風速を総合評価）
- 追加気象データ（風速・風向・気圧・露点・視程）
- 天文薄明・日月出没時刻表示
- 24時間観測適性タイムライン
- ナイトビジョンモード（赤色表示）
- お気に入り地点機能（最大5件）
- 観測適性レーダーチャート
- 天体イベント情報（惑星・流星群・推奨天体）

### Changed
- UIを大幅に刷新し、天体観測に特化したダッシュボードに変更

## [1.5.3] - 2026-01-13

### Removed
- 月の出データを削除

### Changed
- バージョンを復元

## [1.5.1] - 日付不明

### Added
- 日時指定機能を追加
- 週間予報クリック機能を追加

## [1.0.0] - 日付不明

### Added
- 初回リリース
- 基本的な天気ダッシュボード機能
