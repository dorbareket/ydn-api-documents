# StatsPage
StatsPageオブジェクトは、getメソッドの実行結果（全Entityのリスト）を保持します。

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
  <td colspan="8"><a href="../Common/Page.md">Page</a>(inherited)</td>
 </tr>
 <tr>
  <td>totalNumEntries</td>
  <td>xsd:int</td>
  <td>取得される項目の総件数です。</td>
  <td colspan="5"></td>
 </tr>
 <tr>
  <td>Page.Type</td>
  <td>xsd:string</td>
  <td>このインスタンスのPageの サブタイプです。</td>
  <td colspan="5"></td>
 </tr>
 <tr>
  <td colspan="8">StatsPage</td>
 </tr>
  <tr>
  <td>period</td>
  <td><a href="./Period.md">Period</a></td>
  <td>統計情報更新日</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>values</td>
  <td><a href="./StatsValues.md">StatsValues</a> <br>inherited　
  <a href="./CampaignStatsValues.md">CampaignStatsValues</a>
  <br>inherited　
  <a href="./AdGroupStatsValues.md">AdGroupStatsValues</a><br>inherited<br>
  <a href="./AdStatsValues.md">AdStatsValues</a> 
  <br>inherited　
  <a href="./ImageStatsValues.md">ImageStatsValues</a><br>inherited　
  <a href="./VideoStatsValues.md">VideoStatsValues</a><br>inherited　
  <a href="./TargetStatsValues.md">TargetStatsValues</a></td>
  
  <td>getメソッドの実行結果です。</td>
  <td>yes</td>
  <td>-</td>
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
