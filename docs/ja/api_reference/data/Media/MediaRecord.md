# MediaRecord
MediaRecordオブジェクトは、画像の情報を表します。
### Service
+ [MediaService](../../services/MediaService.md)

### Namespace
[MediaService#Namespace](../../services/MediaService.md#namespace)

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
 <tr>
  <td>accountId</td>
  <td>xsd:long</td>
  <td>アカウントIDです。</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Requirement<br>NotUpdatable</td>
  <td>Requirement<br>NotUpdatable</td>
 </tr>
  <tr>
  <td>mediaId</td>
  <td>xsd:long</td>
  <td>画像IDです。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>Requirement<br>NotUpdatable</td>
  <td>Requirement<br>NotUpdatable</td>
 </tr>
  <tr>
  <td>mediaName</td>
  <td>xsd:string</td>
  <td>実ファイル名です。</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>-</td>
  <td>-</td>
 </tr>
  <tr>
  <td>mediaTitle</td>
  <td>xsd:string</td>
  <td>画像名です。</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Optional<br>Updatable</td>
  <td>-</td>
 </tr>
  <tr>
  <td>userStatus</td>
  <td>enum<br><a href="./UserStatus.md">UserStatus</a></td>
  <td>配信状況です。</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>Optional<br>Updatable</td>
  <td>-</td>
 </tr>
   <tr>
  <td>logoFlg</td>
  <td>enum<br><a href="./LogoFlg.md">LogoFlg</a></td>
  <td>ロゴフラグです。（デフォルト：FALSE）</td>
  <td>yes</td>
  <td>-</td>
  <td>Optional</td>
  <td>Optional<br>Updatable</td>
  <td>-</td>
 </tr>
   <tr>
  <td>thumbnailFlg</td>
  <td>enum<br><a href="./ThumbnailFlg.md">ThumbnailFlg</a></td>
  <td>サムネイルフラグです。（デフォルト：FALSE）</td>
  <td>yes</td>
  <td>-</td>
  <td>Optional</td>
  <td>-</td>
  <td>-</td>
 </tr>
  <tr>
  <td>creationTime</td>
  <td>xsd:string</td>
  <td>入稿日時です。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
   <tr>
  <td>approvalStatus</td>
  <td>enum<br><a href="./MediaApprovalStatus.md">MediaApprovalStatus</a></td>
  <td>審査の状況です。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
   <tr>
  <td>disapprovalReasonCodes</td>
  <td>xsd:string</td>
  <td>掲載拒否の理由です。</td>
  <td>yes</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
  <td>-</td>
 </tr>
   <tr>
  <td>media</td>
  <td><a href="./Media.md">Media</a><br>inherited<br><a href="./ImageMedia.md">ImageMedia</a></td>
  <td>画像の設定内容です。</td>
  <td>yes</td>
  <td>-</td>
  <td>Requirement</td>
  <td>-</td>
  <td>-</td>
 </tr>
</table>

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
