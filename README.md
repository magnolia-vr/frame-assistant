# Frame Assistant 0.7.0 preview（試験版）

Steam Frame を PC につないで使うときの便利機能をまとめた、Windows 用の非公式・無料ツールです。

**0.7.0 preview は 2026年10月18日に試験版として公開しました。配布ファイルの組み立て時の検査は済んでいます。実機での確認は進めている途中です。**

0.6.7 から VR メニューを1つにまとめ、時計と5つの色、アナウンス翻訳、注視自動翻訳、曜日アラーム、予約撮影・水平補正、床と位置の調整・手動固定、メモと寝落ち設定を追加しました。独自アイトラと補助ボタンの設定も VR で操作します。

左の一覧は英語だけで、HOME（ホーム）、ANNOUNCE（アナウンス翻訳）、GAZE（視線翻訳）、TIMER（タイマー）、ALARM（アラーム）、SYSTEM（性能）、CAPTURE（撮影）、PLAY AREA（遊ぶ範囲と位置）、SETTINGS（設定）、LAB（ラボ）の10ページです。TIMER はタイマー専用で、音は「TIMER SOUND／タイマーの音・試聴」。アラームの一覧・追加・変更・曜日・ON/OFF・スヌーズ・停止・音の選択は独立した ALARM で行い、音は「ALARM SOUND／アラームの音・試聴」です。

TIMER の「HUD NOTICE／視界への通知」が ON のとき、有効なアラームは時計の左、動作中のタイマーは右の板に出ます。アプリ内通知が OFF でも出ます。板は表示だけで、操作は VR メニューで行います。

まばたきの測定は、SETTINGS（設定）の EYE（アイトラ）→「まばたきの測定」→「測定を始める」から。ふつうに3秒目を開け、ゆっくり10回まばたきして「10回終わった」を押し、結果を見て「保存」します。「前の値に戻す」「調整をやめる」で戻せます。自分で測って保存した値だけを使い、自動学習はしません。効果は使う人ごとに実機で確かめてください。

- [ホームページの公開先](https://magnolia-vr.github.io/frame-assistant/)
- [0.7.0 preview のリリース予定先](https://github.com/magnolia-vr/frame-assistant/releases/tag/v0.7.0-preview)
- [0.7 の動作チェック表](checklist.html)
- [以前の0.6.7試験版](https://github.com/magnolia-vr/frame-assistant/releases/tag/v0.6.7-preview)

配布ファイルは `FrameAssistant-Setup-0.7.0-preview.exe`（106,176,821 バイト、SHA256 `88b5729554b6479b0a042acad3e11c4e00d2dcdfbe48146f148a28ea1b8aaa9b`）と `Frame-Assistant-Setup-0.7.0-preview.zip`（150,036,031 バイト、SHA256 `4e9a354f3c85324e0974b953e2ebbf49c497a569ef2b4d072a13cf76efbcd183`）、タグは `v0.7.0-preview` です。

作者さんのアプリ（sasaken1102r さんの frameeyeosc など）や PC 側の VRCFaceTracking 用の部品は、セットアップが検出し、選んだ対象だけ控え・停止・無効化します。控えから戻せます。共有設定は消しません。新しい VRCFaceTracking 経由の送信は確認が残り、まだ導入できません。

アラームはアプリ終了後に残りません。録画・窓の表示・目合わせは未対応です。音声の言い方のページは0.6.7向けの参考です。使える操作は0.7の画面で確認してください。

このリポジトリはホームページと配布物の公開用です。公開するサイトは許可されたファイルだけに限り、研究記録・控え・目録は含めません。Valve・VRChat とは関係ありません。
