# AuditLogDownloadStatusSelector
getDownloadStatusメソッドの検索条件（実行パラメータ）を保持するオブジェクトです。

### Service
+ [AuditLogService](../../services/AuditLogService.md)

### Namespace
[AuditLogService#Namespace](../../services/AuditLogService.md#namespace)

<table>
 <tr>
  <th>Field</th>
  <th>Type</th>
  <th>Description</th>
  <th>response</th>
  <th>getDownloadStatus</th>
  <th>add</th>
  <th>set</th>
  <th>remove</th>
 </tr>
 <tr>
  <td>accountId</td>
  <td>xsd:long</td>
  <td>アカウントIDです。</td>
  <td>-</td>
  <td>Requirement</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>auditLogJobIds[1...500]</td>
  <td>xsd:long</td>
  <td>ジョブIDです。</td>
  <td>-</td>
  <td>Optional</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>auditLogJobStatuses[1...3]</td>
  <td>enum <br><a href="./AuditLogDownloadJobStatus.md">AuditLogDownloadJobStatus</a></td>
  <td>ジョブステータスです。</td>
  <td>-</td>
  <td>Optional</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
 <tr>
  <td>paging</td>
  <td><a href="../Common/Paging.md">Paging</a></td>
  <td>取得範囲です。</td>
  <td>-</td>
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
