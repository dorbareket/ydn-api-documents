# AdGroupOperation
AdGroupOperationオブジェクトは、操作の対象となる広告グループと処理の内容を表します。
### Service
+ [AdGroupService](../../services/AdGroupService.md)

### Namespace
[AdGroupService#Namespace](../../services/AdGroupService.md#namespace)


| フィールド | データ型 | 説明 | 制限 |
|---|---|---|---|
| Operation(inherited)||||
| operator| enum Operator| 処理を表す演算子です。| Req |
| AdGroup Operation||||
| accountId| xsd:long| アカウントIDです。| Req |
| operand[]| <a href="./AdGroup.md">AdGroup</a>| コンテナです。| Req |

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
