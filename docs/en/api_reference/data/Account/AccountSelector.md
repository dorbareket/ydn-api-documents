# AccountSelector
The AccountSelector object is used to select accounts for acquisition.
### Service
+ [AccountService](../../services/AccountService.md)

### Namespace
[AccountService#Namespace](../../services/AccountService.md#namespace)

| Field | Data Type | Description |
|---|---|---|
| accountIds| xsd: long[]| If nothing is selected, all accounts are retrieved. |
| accountTypes| enum <a href="AccountType.md">AccountType[]</a>| Selects account type. |
| accountStatuses| enum <a href="AccountStatus.md">AccountStatus[]</a>| Selects account status. |
| paging| <a href="../Common/Paging.md">Paging</a>| The page that is returned as a page. |

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
