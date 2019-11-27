

# ReportDateRangeType (enum)

ReportDateRangeTypeは、レポートの集計対象期間を表します。

#### Service

+ [ReportDefinitionService](../../services/ReportDefinitionService.md)

#### Namespace

[ReportDefinitionService#Namespace](../../services/ReportDefinitionService.md#namespace)

| Enumeration  |       Type       |          Description          |
| ------------ | ---------------- | ----------------------------- |
| CUSTOM_DATE | xsd:string | ユーザーにより指定される期間です。CUSTOM_DATEを指定した場合、集計対象期間の指定が必要です。<br>※ReportType : REACHでは指定不可 |
| YESTERDAY | xsd:string | 昨日です。 |
| LAST_7_DAYS | xsd:string | 本日を除く、過去7日間です。 |
| LAST_WEEK | xsd:string | 先週の月曜日から日曜日です。 |
| LAST_BUSINESS_WEEK | xsd:string | 先週の月曜日から5営業日です。 |
| LAST_14_DAYS | xsd:string | 本日を除く、過去14日間です。 |
| LAST_30_DAYS | xsd:string | 本日を除く、過去30日間です。 |
| THIS_MONTH | xsd:string | 本日を除く、当月です。 |
| LAST_MONTH | xsd:string | 前月です。 |

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
