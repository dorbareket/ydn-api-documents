# ReturnValue
ReturnValueオブジェクトは、処理の結果を表します。
### Service
全サービス共通

| フィールド | データ型 | 説明 | 制限 |
|---|---|---|---|
| operationSucceeded| xsd: boolean| 処理結果です。trueの場合は、処理は成功しました。falseの場合は処理が失敗しています。| Req |
| error| <a href="Error.md">Error[]</a>| エラー内容です。| Opt |

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
