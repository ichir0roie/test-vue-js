

https://v3.vuejs.org/guide/introduction.html#getting-started


# カウンター機能

色々やってみた結果、
export defaultに直接メソッドとか変数を設定したらうまく行ったようだ。
詳しいことは把握していないが、おそらく default メソッドがconst any や new Vue()などの木うのと同様の仕様になっているのだろう。

つまり、スタート地点はともかく、
開始方法はいくつかあり、
+ const valuible
+ new Vue()
+ export default

など、複数地点からのオブジェクトの記述方法があるようだ、。k
パッケージ等を使用した場合の実装方法にはブレがあるかもしれないが、概ねここからとっかかっていけば良いのではないだろうか。

