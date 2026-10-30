# 橋の固有振動数

スマホの加速度センサーで、歩道橋・道路橋の固有振動数を測る 1 枚の Web ページ。

- 公開 URL: https://koshi-san.github.io/bridge-frequency/
- 「このスマホで計測」で直接記録（HTTPS で開いた Android Chrome などで動作）
- phyphox の CSV も読み込み可
- 等間隔に補間 → 線形トレンド除去 → Hann 窓 → Welch 法でスペクトルを求め、上位 3 ピークを表示
- 歩行の振動数帯 1.5–2.3 Hz と、経験式 f ≈ 100/L の目安を重ねて表示
