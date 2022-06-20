# ai-robot-chapter3
- 注意事項
  - 実行するUbuntuの環境でマイクからの音声入力とスピーカーからの音の出力が出来ていることを事前に確認してください。
  - バーチャルマシン上のUbuntuを使用する場合は、遅れが生じて音声が出力されない事があります。長めの発話文を入力するなどして対応して下さい。
  - 可能であればベッドセットを使用してください。オウム返しの実行中にスピーカーの音がマイクに回って繰り返す場合があります。
- 3.1 音声認識の実行手順
- 3.2 音声合成の実行手順
  - ros2 topic pub -1 /speech std_msgs/msg/String "{data: 'I will go to the kitchen and grab a bottle.'}"
  - 困ったとき
    - 音声がスピーカーから出力されない場合は、synthesis_mpg123.pyからの実行を試してください。音声合成されたmp3ファイルが出力されるので、そのファイルを再生して確認してください。
- 3.3.1 トピック通信によるオウム返しの実行手順
- 3.3.2 サービスによるオウム返しの実行手順
  - 困ったとき
    - 音声がスピーカーから出力されない場合は、speech_service_mpg123.pyからの実行を試してください。音声合成されたmp3ファイルが出力されるので、そのファイルを再生して確認してください。
