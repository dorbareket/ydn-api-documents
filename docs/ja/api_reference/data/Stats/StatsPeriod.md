

# StatsPeriod (enum)

StatsPeriodは、統計情報の集計期間を表します。

#### Service

+ [StatsService](../../services/StatsService.md)

#### Namespace

[StatsService#Namespace](../../services/StatsService.md#namespace)

| Enumeration  |       Type       |          Description          |
| ------------ | ---------------- | ----------------------------- |
| REALTIME_TODAY | xsd:string | 今日 / 速報値 |
| DEFINITE_VALUE_YESTERDAY | xsd:string | 昨日 / 確定値 |
| DEFINITE_VALUE_LASTWEEK | xsd:string | 先週（月-日）/ 確定値 |
| DEFINITE_VALUE_LASTBSDAY | xsd:string | 先週（月-金）/ 確定値 |
| DEFINITE_VALUE_WEEK | xsd:string | 過去7日間（今日を含まない）/ 確定値 |
| DEFINITE_VALUE_TWOWEEK | xsd:string | 過去14日間（今日を含まない）/ 確定値 |
| DEFINITE_VALUE_THIRTYDAY | xsd:string | 過去30日間（今日を含まない）/ 確定値 |
| REALTIME_MONTH | xsd:string | 今月（今日を含む）/ 速報値 |
| DEFINITE_VALUE_LASTMONTH | xsd:string | 先月 / 確定値 |
| DEFINITE_VALUE_LAST13MONTH | xsd:string | 過去13ヶ月間 / 確定値 |
| CUSTOM_DATE | xsd:string | 任意日付の指定 |

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
