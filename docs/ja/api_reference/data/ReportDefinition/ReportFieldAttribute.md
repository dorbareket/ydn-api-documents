

# ReportFieldAttribute

ReportFieldAttributeは、getReportFieldsメソッドの実行結果（１FieldEntity）を保持するオブジェクトです。

### Service

+ [ReportDefinitionService](../../services/ReportDefinitionService.md)

### Namespace

[ReportDefinitionService#Namespace](../../services/ReportDefinitionService.md#namespace)

| Field | Type | Description | response |
| ----- | ---- | ----------- | -------- |
| fieldName | xsd:string | フィールド名 | yes | |
| displayFieldNameJA | xsd:string | ダウンロードされたレポートに表示されるフィールド名（日本語） | yes | |
| displayFieldNameEN | xsd:string | ダウンロードされたレポートに表示されるフィールド名（英語） | yes | |
| xmlAttributeName | xsd:string | ダウンロードしたレポートのXML属性 | yes | |
| fieldType | xsd:string | フィールドタイプ（数字、文字列、ENUM値など） | yes | |
| filterable | xsd:boolean | フィールドのフィルター指定可否（true：フィルター指定可能なフィールド） | yes | |
| impossibleCombinationFields | xsd:string | 組み合わせ不可フィールド | yes | |

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
