
# これはなんですか?

メタトレーダー5用のEAです

# インストール方法

1. こちらのリンクからXMtradingに登録してください。 <a href="https://clicks.affstrack.com/c?c=574014&l=ja&p=0">XMtrading</a> 口座タイプはスタンダードがおすすめです。
1. こちらからXMtrading用のMetaTrader5をダウンロードしてインストールしてください。 <a href="https://clicks.affstrack.com/c?c=574014&l=ja&p=4">MetaTrader 5</a>
1. こちらのファイルをMetaTrader5のEA用のディレクトリに設置してください。 [PhaseShift.ex5](PhaseShift.ex5) 
1. 通貨は USDJPY そして チャートは 1分足(M1)を設定してください。
1. <b>XMTrading MT5</b> を起動してください。
1. ツール => オプション => 『WebRequestを許可するURLリスト』 に 新しいURLを追加する、から次のURLを追加してください。
 `https://jw0tzq2rp3.execute-api.ap-northeast-1.amazonaws.com`

# パラメータ

| パラメータ名 | 意味 |
|--|--|
|EA_Magic| マジックナンバー |
|Lot|1度の注文で使うロット数|
|StopLoss|ストップロス(%)|
|TakeProfit|テイクプロフィット(%)|
|ResetProfit|リセットプロフィット(%) <small>(※1)</small>|
|MaPeriod|Moving Average（移動平均線）指標を計算する期間|
|AdxPeriod|ADX (Average Directional Movement ）指標を計算する期間|
|TradeWait|同じマジックナンバーで次の注文を行うまでの待ち時間  <small>(※2)</small>|
|SellAdx|売り注文時に判断するADXの値|
|BuyAdx|回注文時に判断するADXの値|

#### ※1 Profitがこの値を下回ったら利益の出る可能性が低い注文としてTakeProfitを買値/売値と同じにしてTakeProfit０にしProfitが0になった瞬間そのポジションは閉じられる
####  ※2 同じマジックナンバーでも買注文と売注文は区別するため、wait中でも同時に注文できる


# 問い合わせや不具合について

このリポジトリの <a href="https://github.com/kiyomasa-sato-0519/PhaseShift/issues">issues</a> をご利用ください

# 免責について

リスクは自己責任でお願いします。
