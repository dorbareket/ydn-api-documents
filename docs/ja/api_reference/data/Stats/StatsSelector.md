# StatsSelector
StatsSelectorオブジェクトは、getメソッドの検索条件（実行パラメータ）を保持します。

### Service
+ [StatsService](../../services/StatsService.md)

### Namespace
[StatsService#Namespace](../../services/StatsService.md#namespace)

<table>
 <tr>
  <th>Field</th>
  <th>Type</th>
  <th>Description</th>
  <th>response</th>
  <th>get</th>
  <th>add</th>
  <th>set</th>
  <th>remove</th>
 </tr>
 <tr>
  <td>accountId</td>
  <td>xsd:long</td>
  <td>アカウントID</td>
  <td>yes</td>
  <td>Requirement</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>campaignIds[0...500]</td>
  <td>xsd:long</td>
  <td>キャンペーンID<br>statsTypeで「CAMPAIGN」または「ADGROUP」または「AD」または「TARGET」を指定した場合のみ有効です。</td>
  <td>yes</td>
  <td>Optional</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>adGroupIds[0..500]</td>
  <td>xsd:long</td>
  <td>広告グループID<br>statsTypeで「ADGROUP」または「AD」または「TARGET」を指定した場合のみ有効です。</td>
  <td>yes</td>
  <td>Optional</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>adIds[0..500]</td>
  <td>xsd:long</td>
  <td>広告ID<br>statsTypeで「AD」を指定した場合のみ有効です。</td>
  <td>yes</td>
  <td>Optional</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>medialds[0..500]</td>
  <td>xsd:long</td>
  <td>画像ID<br>statsTypeで「MEDIA」を指定した場合のみ有効です。</td>
  <td>yes</td>
  <td>Optional</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>targetTypes[0..1]</td>
  <td>enum<br>
  <a href="./TargetType.md">TargetType</a></td>
  <td>ターゲットタイプ<br>statsTypeで「TARGET」を指定した場合のみ必須です。</td>
  <td>yes</td>
  <td>Optional</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>statsPeriod</td>
  <td>enum<br>
  <a href="./StatsPeriod.md">StatsPeriod</a></td>
  <td>統計情報の集計期間<br>デフォルトでは「REALTIME_MONTH」に設定されています。</td>
  <td>yes</td>
  <td>Optional</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
  <tr>
  <td>statsPeriodCustomDate</td>
  <td><a href="./StatsPeriodCustomDate.md">StatsPeriodCustomDate</a></td>
  <td>統計情報の集計期間<br>年月日で指定可能です。<br>StatsPeriodが「CUSTOM_DATE」の時は入力が必須です。</td>
  <td>yes</td>
  <td>Optional</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>statsType</td>
  <td>enum<br>
  <a href="./StatsType.md">StatsType</a></td>
  <td>統計情報の種別<br>デフォルトでは「CAMPAIGN」に設定されています。</td>
  <td>yes</td>
  <td>Optional</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>paging</td>
  <td><a href="../Common/Paging.md">Paging</a></td>
  <td>ページ設定情報</td>
  <td>yes</td>
  <td>Optional</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
</table>

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">
<img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" />
</a><br />
この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">
クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
