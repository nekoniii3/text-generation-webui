# Text-generation-webUI用Colabノート
 Text-generation-webUIを使うためのGoogleColabノートブックです。<br>
基のリポジトリはこちら→[Text generation web UI](https://github.com/oobabooga/text-generation-webui)
<br><br>

## 利用方法

①～③までの再生マークを順に実行し、表示される"http://～.gradio.live"をクリックして実行して下さい。<br>
(Stable Diffusion WebUIのような感じです）
<br><br>

最初にランタイムをGPUに変更
![](images/s-1-1.png)

無料版は[T4 GPU]に<br>
※JapaneseStableLMはA100でしか動作確認できてません。（有料版のみ選択可能）
![](images/1-2.png)



## 注意
・JapaneseStableLMはGoogleColab有料版で利用できるGPU:A100でのみ動作が確認できています。<br>
（無料版では厳しいと思います）<br>
・初期設定でキャラクターがつけてある場合があるので適宜設定して下さい。<br>
（日本語で設定すると、回答も日本語になる可能性が上がります）


## 補足
JapaneseStableLMはそのままだと動作しなかったため、models.pyを修正しています。<br>
（tokenizerを"novelai/nerdstash-tokenizer-v1"にしています。）

## 利用させて頂いたリポジトリ・モデルファイルなど

・JapaneseStableLMモデルファイル<br>
https://huggingface.co/stabilityai/japanese-stablelm-base-alpha-7b/tree/main
<br><br>
・japanese-large-lmモデルファイル<br>
https://huggingface.co/line-corporation/japanese-large-lm-3.6b/tree/main