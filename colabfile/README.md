# Text-generation-webUI用Colabノート
 Text-generation-webUIを使うためのGoogleColabノートブックです。<br>
基のリポジトリはこちら→[Text generation web UI](https://github.com/oobabooga/text-generation-webui)
<br><br>

## 利用方法

①～③までの再生マークを順に実行し、表示される"http://～.gradio.live"をクリックして実行して下さい。<br>
(Stable Diffusion WebUIのような感じです）
<br><br>

最初にランタイムをGPUに変更
![](images/1-1.png)

無料版は[T4 GPU]に<br>
※JapaneseStableLMは[A100]でしか動作確認できてません。（有料版のみ選択可能）
![](images/1-2.png)

①の再生マークをクリック（終了まで3分程度かかります）
![](images/1-3.png)

②の再生マークをクリック（終了まで3分程度かかります）
![](images/1-4.png)

③の再生マークをクリック
![](images/1-5.png)

"http://～.gradio.live"をクリック（URLが出てくるまで3分程度かかります）
![](images/1-6.png)

## 注意
・JapaneseStableLMはGoogleColab有料版で利用できるGPU:A100でのみ動作が確認できています。<br>
・初期設定でキャラクターがついてある場合があるので適宜設定して下さい。<br>
（日本語で設定すると、回答も日本語になる可能性が上がります）


![](images/2-1.png)


## 補足
JapaneseStableLMはそのままだと動作しなかったため、models.pyを修正しています。<br>
（tokenizerを"novelai/nerdstash-tokenizer-v1"にしています。）

## 利用させて頂いたリポジトリ・モデルファイルなど

・JapaneseStableLMモデルファイル<br>
https://huggingface.co/stabilityai/japanese-stablelm-base-alpha-7b/tree/main
<br><br>
・japanese-large-lmモデルファイル<br>
https://huggingface.co/line-corporation/japanese-large-lm-3.6b/tree/main