# ManualCPVAdGroupAdBid
ManualCPVAdGroupAdBid object displays the manual bidding method for ad (CPV).
※This information is available only when a campaign ID with ad distribution type 'VIDEO_AD' is specified.

### Service
+ [AdGroupAdService](../../services/AdGroupAdService.md)

### Namespace
[AdGroupAdService#Namespace](../../services/AdGroupAdService.md#namespace)

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
  <td>type</td>
  <td>enum<br><a href="./BiddingStrategyType.md">BiddingStrategyType</a></td>
  <td>Bidding method.</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Ignore<br>NotUpdatable</td>
  <td>Ignore<br>NotUpdatable</td>
 </tr>
 <tr>
  <td>maxCpv</td>
  <td>xsd:long</td>
  <td>Bid amount</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Optional<br>Updatable</td>
  <td>Ignore<br>NotUpdatable</td>
 </tr>
</table>

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
