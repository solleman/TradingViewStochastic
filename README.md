# TradingViewStochastic

TradingViewStochastic

three classes : 

TradingViewStochastic.java
StochasticOscillatorKIndicator2.java
StochasticOscillatorKIndicator2.java

Example :


  ClosePriceIndicator closeIndicator = new ClosePriceIndicator(series);
  RSIIndicator rsi = new RSIIndicator(closeIndicator, 14);

  TradingViewStochastic tvs = new TradingViewStochastic(rsi, 14, rsi, rsi);
  StochasticOscillatorKIndicator2 stok = new StochasticOscillatorKIndicator2(tvs);
  StochasticOscillatorDIndicator2 stod = new StochasticOscillatorDIndicator2(stok);

  System.out.println("stok  : " + stok.getValue(series.getEndIndex()));
	System.out.println("stod  : " + stod.getValue(series.getEndIndex()));
