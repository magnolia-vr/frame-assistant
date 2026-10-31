# Orbit System（Frame Assistant）0.7.3 preview（試験版）

Steam Frame を PC につないで使うときの便利機能をまとめた、Windows 用の非公式・無料ツールです。

**0.7.3 preview は 2026年10月31日に試験版として公開しました。配布ファイルの組み立て時の検査は済んでいます。実機での確認は進めている途中です。**

0.6.7 から VR メニューを1つにまとめ、時計と5つの色、アナウンス翻訳、注視自動翻訳、曜日アラーム、予約撮影・水平補正、床と位置の調整・手動固定、メモと寝落ち設定を追加しました。独自アイトラと補助ボタンの設定も VR で操作します。

0.7.3 では、Frame の初期化後に部品がすべて消えている場合の入れ直しと VR メニューの接続を直し、通知・HUD の配置・手の甲の操作パネルを変更しました。PC マイクのミュートなどを削除し、白いブラウザの板が自動で開かないようにしました。アンインストールは模擬の試験までです。

0.7.2 では、VR メニューの選んだ枠のずれを直し、視界の HUD の配置を Frame だけで変えられるようにし（アラーム・タイマーの板は時計と一緒に動きます）、空間のキーボードの種類とコピー・貼り付け、指先の操作（試し）、スクショ・録画を PC のピクチャ／ビデオの「Orbit System」へ自動で送る形（件数の上限なし）、タイマー・アラームの音、SteamVR が起動し直したあとの PlaySpace の復帰、Frame を初期化したあとの登録し直し、アンインストーラーを加えました。VR のブラウザは準備中です。

0.7.1 では、PC アプリの画面を VR メニューと同じ見た目（左の一覧12ページ・2列カード）に作り直し、Discord の通知を Frame の視界に出す機能（最初から ON）、VRChat で会った人の記録と印（最初は OFF）、移動に使う手と戻す長押しの秒数の設定、Frame の住所が変わったときの探し直しを加えました。アプリ内の通知は最初から ON です。

左の一覧は英語だけで、HOME（ホーム）、ANNOUNCE（アナウンス翻訳）、GAZE（視線翻訳）、TIMER（タイマー）、ALARM（アラーム）、SYSTEM（性能）、CAPTURE（撮影）、PLAY AREA（遊ぶ範囲と位置）、SETTINGS（設定）、LAB（ラボ）の10ページです。TIMER はタイマー専用で、音は「TIMER SOUND／タイマーの音・試聴」。アラームの一覧・追加・変更・曜日・ON/OFF・スヌーズ・停止・音の選択は独立した ALARM で行い、音は「ALARM SOUND／アラームの音・試聴」です。

TIMER の「HUD NOTICE／視界への通知」が ON のとき、有効なアラームは時計の左、動作中のタイマーは右の板に出ます。アプリ内通知が OFF でも出ます。板は表示だけで、操作は VR メニューで行います。

まばたきの測定は、SETTINGS（設定）の EYE（アイトラ）→「まばたきの測定」→「測定を始める」から。ふつうに3秒目を開け、ゆっくり10回まばたきして「10回終わった」を押し、結果を見て「保存」します。「前の値に戻す」「調整をやめる」で戻せます。自分で測って保存した値だけを使い、自動学習はしません。効果は使う人ごとに実機で確かめてください。

- [ホームページの公開先](https://magnolia-vr.github.io/frame-assistant/)
- [0.7.3 preview のリリース](https://github.com/magnolia-vr/frame-assistant/releases/tag/v0.7.3-preview)
- [0.7.2 preview のリリース](https://github.com/magnolia-vr/frame-assistant/releases/tag/v0.7.2-preview)
- [0.7.1 preview のリリース](https://github.com/magnolia-vr/frame-assistant/releases/tag/v0.7.1-preview)
- [0.7.0 preview のリリース](https://github.com/magnolia-vr/frame-assistant/releases/tag/v0.7.0-preview)
- [0.7 の動作チェック表](checklist.html)
- [以前の0.6.7試験版](https://github.com/magnolia-vr/frame-assistant/releases/tag/v0.6.7-preview)

配布ファイルは `FrameAssistant-Setup-0.7.3-preview.exe`（350,902,427 バイト、SHA256 `68e8991e84f84f0b77e9d8164d785ced3ed8d87e8a1ec8c6089d8367bd4ed33d`）と `Frame-Assistant-Setup-0.7.3-preview.zip`（488,975,079 バイト、SHA256 `5ad5ae370433f4797edc37f27ded9f9378a9383a65459541a314cf4e40069eed`）、タグは `v0.7.3-preview` です。

作者さんのアプリ（sasaken1102r さんの frameeyeosc など）や PC 側の VRCFaceTracking 用の部品は、セットアップが検出し、選んだ対象だけ控え・停止・無効化します。控えから戻せます。共有設定は消しません。新しい VRCFaceTracking 経由の送信は確認が残り、まだ導入できません。

アラームはアプリ終了後に残りません。写真・動画を PC の好きなフォルダーへ保存する機能は次の版の予定です。窓の表示・目合わせは未対応です。音声の言い方のページは0.6.7向けの参考です。使える操作は0.7の画面で確認してください。

このリポジトリはホームページと配布物の公開用です。公開するサイトは許可されたファイルだけに限り、研究記録・控え・目録は含めません。Valve・VRChat とは関係ありません。

時計HUD・SYSTEMの電池残量はSteamVRを優先します。PCの電池予測・20%/10%通知は本体内部の値を使うため、表示とずれることがあります。
声の撮影は、全体電源と音声待受をONにし、起動ごとにPCの「スクショ・録画」で対象の視線・音声をONにして、Frame側の撮影準備を整えて使います。拒否理由の案内と、個別OFF後の録画停止を修正しました。
