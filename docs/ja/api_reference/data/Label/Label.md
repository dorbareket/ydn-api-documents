# Label
Labelオブジェクトは、ラベルの情報を表します。

### Service
+ [LabelService](../../services/LabelService.md)

### Namespace
[LabelService#Namespace](../../services/LabelService.md#namespace)

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
  <td>accountId</td>
  <td>xsd:long</td>
  <td>アカウントID</td>
  <td>yes</td>
  <td>Ignore</td>
  <td>Ignore</td>
  <td>Ignore</td>
 </tr>
 <tr>
  <td>labelId</td>
  <td>xsd:long</td>
  <td>ラベルID</td>
  <td>yes</td>
  <td>Ignore</td>
  <td>Requirement</td>
  <td>Requirement</td>
 </tr>
 <tr>
  <td>labelName</td>
  <td>xsd:string</td>
  <td>ラベル名</td>
  <td>yes</td>
  <td>Requirement</td>
  <td>Optional</td>
  <td>Ignore</td>
 </tr>
 <tr>
  <td>color</td>
  <td>xsd:string</td>
  <td>カラー</td>
  <td>yes</td>
  <td>Optional<br>※default: #FFFFFF</td>
  <td>Optional</td>
  <td>Ignore</td>
 </tr>
  <tr>
  <td>description</td>
  <td>xsd:string</td>
  <td>説明文</td>
  <td>yes</td>
  <td>Optional</td>
  <td>Optional</td>
  <td>Ignore</td>
 </tr>
</table>

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
