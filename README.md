# Seoul Air Quality Prediction

# 1. テーマ

ソウルのPM10とPM2.5を予測するマシンラーニング

中国ペキンの大気汚染濃度データをもとにして
韓国ソウルの大気汚染濃度を予測する事を目標にする。

중국 베이징의 대기오염 농도 데이터를 기반으로 하여
서울의 대기오염 농도를 예측하는 것을 목표로 한다

# 2. 企画、目標

現代人にとってPM2.5は重要な事案になった。
最近PM2.5の危険性に関する研究を見るとPM2.5は呼吸器、循環器病だけではなく癌、精神病、肥満など様々な病気に影響を及ぼしており
みんなの敵だとも呼ぶことができる。
よって、毎日変化して行く韓国の大気汚染濃度を知ることはとても重要だ。

現在ソウルの大気汚染はかなり深刻な状況だ。
一方、ソウルの大気汚染は中国からくるPM2.5が主な原因だという事実は広く知れている。
よって、韓国の大気汚染の原因である中国からPM2.5を測定しそのデータを分析したらソウルのPM2.5濃度も大雑把に予測する事ができるはずだ。

ただし風速、風向も考えて予測する事を建て前にしながら一年周期で予測する事を目標にする。

風速、風向によって些細な差があるかもしれないが普通中国から韓国までPM2.5が来るには平均的に一日ぐらいかかる。
そんな事実から考えると中国でPM2.5を測定した後そのデータを知ることができたら韓国の明日のPM2.5を予測する事が出来るようになるし
予測PM2.5数値に従って適切な処置を予めすることもできるようになるはずだ。

ここでは明日の大気汚染濃度を予測する事を目標にしているがもっと多いデータを収集、分析することができるようになったら
一年後または二年後の大気汚染濃度も予測する事が出来るはずだ。
究極的には韓国の大気汚染を減らす方法を探す資料として活用されることを目指している。


ソウルはPM10とPM2.5で悩まされ、外出するすると必ずマスクをつけるようになりました。韓国の国内で発生したものだとしたら、四季によることは少ないことが当然ですが、冬と春はひどく濃いPM2.5で、中国を疑っています。

それで、私たちは北京とソウルの空気のデータを使い、ソウルの一年間のPM10とPM2.5の予報が出来るようにするとともにどのくらい中国からの影響があるのか試してみようとしております。



현대인들에게 있어서 미세먼지는 중요한 사안이 되었다.
최근 미세먼지 위험성 연구를 살펴보면 미세먼지는 비단 호흡기, 심혈관 질환뿐만 아니라
암, 정신 질환, 비만 등 여러 질환에 영향을 미치고 있으며 가히 공공의 적이라고 부를 만하다
따라서 매일마다 달라지는 한국의 대기오염 농도를 아는 것은 매우 중요하다

현재 서울의 대기오염은 매우 심각한 상황이다
한편, 서울의 대기오염은 중국으로부터 넘어오는 미세먼지가 주된 원인이라고 알려져 있다
따라서 한국 대기오염의 주된 원인인 중국에서의 미세먼지를 측정하여
그 데이터를 분석한다면 서울의 미세먼지 농도도 대략적으로 유추할 수 있을 것이다

단 풍속, 풍향도 고려해서 예측하는 것을 원칙으로 하며
1년주기로 예측하는 것을 목표로 한다

풍속, 풍향에 따라 약간의 차이가 있을 수는 있겠지만
보통 중국에서 한국까지 미세먼지가 넘어오는 데에는 평균적으로 1일정도가 걸린다
그런 사실에 입각하여 생각해본다면 중국에서 미세먼지를 측정한 후
해당 데이터를 알 수 있다면 한국의 1일 뒤의 미세먼지를 예측할 수 있게 되고
그에따른 적절한 조치를 미리 취할 수 있게 될 것이다

지금은 하루 뒤의 대기오염 농도를 예측하는 것을 목표로 하고 있지만
더 많은 데이터를 수집, 분석할 수 있게 된다면
나아가 1년 혹은 2년뒤의 대기오염 농도도 예측할 수 있을 것이다
궁극적으로는 한국의 대기오염을 줄일 수 있는 방법을 찾는 자료로써
활용되는 것을 목표로 하고 있다



# 3. 機能

風速や風向、日付を入力し、その日のPM10とPM2.5を予報する機能

# 4. 開発の環境と流れ

## 4. 1. 環境

- 使用言語：Python
- フレームワーク：Tensorflow, Keras, Seabon, Numpy, Pandasなど
- ツール：Google Colab

## 4. 2. 流れ

1. 試料の調査
2. データの処理
3. モデリング
4. 予測
5. 評価
6. 視覚化

# 5.メンバー

- オ·ソクヒョン
- イ·ハンギョル
- ジョン·ハヨン

# 6. 結論
大韓民国のPM10とPM2.5は、中国で発生したものの影響を受けると推測され、上のようなソウルの空気質を予測する機械学習プロジェクトを実施しました。  
  
初期には北京の空気質、風向、風速のデータとソウルの空気質、風向、風速のデータのみを利用して予測を行いました。 この時北京から韓国まで空気の対流が到達する時間を考慮し、北京のデータは前日のデータと結合して学習を行いました。  
  
その結果、北京とソウルだけのデータで学習させた場合、予測の正確度が落ちる傾向を示しました。 これにより、中国の空気質に大きな影響を受けるペクリョン島の空気質、風向、風速のデータを追加することを決め、3つの地域のデータセットを利用して学習させた結果、予測の数値と実測の数値の差はありましたが、グラフの傾向は一致しました。
  
PM2.5の移動は対流現象と密接に関連しているため、機械学習だけでは中国の影響が大きいという結論を導き出す直接的な根拠にはなりませんが、一つの補助根拠として使われるものと判断され、中国のPM2.5程度によっては、韓国のPM2.5警報の発令を事前に実施できるものと判断されます。  
  
現在のプロジェクトの後の課題としては中国の協力をもらい、北京より大きな影響を与えると疑上海などの空気質、風向、風速のデータを提供してもらって、また、モデリングすることで機械学習の正確度を高めていくことが出来ると判断されております。  
  
대한민국의 미세먼지는 중국에서 만들어진 미세먼지에 영향을 받는다고 추측되어 위와 같은 서울의 공기질 예측 기계학습 프로젝트를 실시하였다.  
  
초기에는 베이징의 공기질, 풍향, 풍속 데이터와 서울의 공기질, 풍향, 풍속 데이터만을 이용하여 예측을 실시하였다. 이 때 베이징으로부터 대한민국까지 공기의 흐름이 도달하는 시간을 고려하여 베이징의 데이터는 하루 전 데이터와 결합하여 학습을 실시하였다.  
  
그 결과 베이징과 서울만의 데이터로 학습시킨 경우 예측도가 떨어지는 경향을 보였다. 이에 따라 중국의 공기질에 큰 영향을 받는 백령도의 공기질, 풍향, 풍속 데이터를 추가하기로 결정하였고 세 지역의 데이터셋을 이용하여 학습시킨 결과 예측과 실측의 값 자체는 차이를 보였으나 경향성이 일치하는 결과를 보여주었다.  
  
미세먼지의 이동은 대류현상과 밀접한 연관이 있기에, 기계학습 만으로는 중국의 영향이 지대하다는 결론을 도출할 직접적인 근거가 될 수는 없으나 하나의 보조근거로서 쓰일 수 있을 것으로 판단되고 중국의 미세먼지 정도에 따라 대한민국의 미세먼지경보 발령을 사전에 실시할 수 있을 것으로 판단된다.  
  
현 프로젝트의 보충과제로서는 중국과의 협력을 통해 베이징 이외의 실제로는 더 큰 영향을 줄 것으로 사료되는 상하이 등의 공기질, 풍향, 풍속 데이터를 제공받아 모델링하는 것으로 기계학습의 정확도를 높여줄 것으로 판단된다.  

# 7. 参考資料

## 7. 1. （韓国）ソウルのデータ

[http://www.airkorea.or.kr/web/realSearch?pMENU_NO=97](http://www.airkorea.or.kr/web/realSearch?pMENU_NO=97)

[https://data.kma.go.kr/data/grnd/selectAsosRltmList.do?pgmNo=36](https://data.kma.go.kr/data/grnd/selectAsosRltmList.do?pgmNo=36)

## 7. 2. （中国）北京のデータ

[https://www.kaggle.com/joshuapaulbarnard/beijing-air-quality-pm25-from-2010-to-2017](https://www.kaggle.com/joshuapaulbarnard/beijing-air-quality-pm25-from-2010-to-2017)

# 8. Colab Link

https://colab.research.google.com/drive/1Jj0f2csbn4WY9tczW3a3D_Sp_PeEXMBm?usp=sharing

# 9. Organizational Tree / 工程図

https://docs.google.com/spreadsheets/d/1RqLtZJ1M8yqnLTpCotfDvekLOfUnD6Mar08XbPVr6CY/edit?usp=sharing
