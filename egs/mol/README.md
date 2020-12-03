### 実験手順

1. LJSpeechをダウンロードし,LJSpeech-1.1をこのディレクトリに置く. (run.shで変更可能)

2. ```
   ./run.sh --stage 0 --stop-stage 0
   ```

   を実行する./data/dev, ./data/eval, ./data/train_no_devが作られ,wavファイルがランダムに配置される

3. ```
   ./run.sh --stage 1 --stop-stage 1
   ```

   を実行する. ./dump/lj/logmelspectrogram/norm/が内に前処理されたwavとmel-spectrogramがnpy形式で配置される. mel-spectrogramをppgに置き換える.

4. ./prepare_ppg_feats.ipynbを実行する

