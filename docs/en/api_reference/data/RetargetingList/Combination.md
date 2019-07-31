# Combination
Combination object is a container for storing combination of target list informarion.
### Service
+ [RetargetingListService](../../services/RetargetingListService.md)

### Namespace
[RetargetingListService#Namespace](../../services/RetargetingListService.md#namespace)

<table>
 <tr>
  <th>Field</th>
  <th>Type</th>
  <th>Description</th>
  <th>response</th>
  <th>add</th>
  <th>set</th>
  <th>remove</th>
 </tr>
 <tr>
  <td>logicalOperator</td>
  <td>enum <a href="./LogicalOperator.md">LogicalOperator</a></td>
  <td>Type of condition for target list.</td>
  <td>yes</td>
  <td>Requirement</td>
  <td>Requirement<br>Updatable</td>
  <td>Ignore</td>
 </tr>
 <tr>
  <td>targetLists[0...n]</td>
  <td><a href="./TargetListData.md">TargetListData</a></td>
  <td>Data of target list.</td>
  <td>yes</td>
  <td>Requirement</td>
  <td>Requirement<br>Updatable</td>
  <td>Ignore</td>
 </tr>
 </table>

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
