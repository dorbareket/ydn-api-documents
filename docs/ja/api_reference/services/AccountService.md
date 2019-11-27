# AccountService

AccountServiceは、アカウントの操作を提供します。

#### WSDL

| environment |                                      url                                      |
| ----------- | ----------------------------------------------------------------------------- |
| production  | https://location.im.yahooapis.jp/services/V201911/AccountService?wsdl |
| sandbox     | https://sandbox.im.yahooapis.jp/services/V201911/AccountService?wsdl  |

#### Namespace

http://im.yahooapis.jp/V201911/Account

#### Service Overview

管理するアカウント情報の取得と更新を行います。

#### Operation

AccountServiceで提供される操作を説明します。

+ [get](#get)
+ [mutate(SET)](#mutateset)

## get

### リクエスト

アカウントの情報を取得します。<br>通常認証ではselectorを省略可です。

| パラメータ | 必須 | データ型 |
| ---------- | ---- | -------- |
| selector | Yes | [AccountSelector](../data/Account/AccountSelector.md) |

##### ＜リクエストサンプル＞
```xml
<SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/">
  <SOAP-ENV:Header>
    <RequestHeader xmlns="http://im.yahooapis.jp/V201911/Account" xmlns:ns2="http://im.yahooapis.jp/V201911">
      <ns2:license>1111-1111-1111-1111</ns2:license>
      <ns2:apiAccountId>2222-2222-2222-2222</ns2:apiAccountId>
      <ns2:apiAccountPassword>password</ns2:apiAccountPassword>
    </RequestHeader>
  </SOAP-ENV:Header>
  <SOAP-ENV:Body>
    <get xmlns="http://im.yahooapis.jp/V201911/Account" xmlns:ns2="http://im.yahooapis.jp/V201911">
      <selector>
        <accountIds>1111</accountIds>
        <accountIds>2222</accountIds>
        <accountIds>3333</accountIds>
        <accountTypes>PREPAY</accountTypes>
        <accountTypes>INVOICE</accountTypes>
        <accountStatuses>INPROGRESS</accountStatuses>
        <accountStatuses>WAIT_DECIDE</accountStatuses>
        <accountStatuses>SUSPENDED</accountStatuses>
        <accountStatuses>SERVING</accountStatuses>
        <accountStatuses>ENDED</accountStatuses>
        <accountStatuses>CANCELED</accountStatuses>
        <paging>
          <ns2:startIndex>1</ns2:startIndex>
          <ns2:numberResults>10</ns2:numberResults>
        </paging>
      </selector>
    </get>
  </SOAP-ENV:Body>
</SOAP-ENV:Envelope>
```

### レスポンス

| パラメータ | データ型 |
| -------- | ------- |
| rval | [AccountPage](../data/Account/AccountPage.md) |

##### ＜レスポンスサンプル＞
```xml
<SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/">
  <SOAP-ENV:Header>
    <ResponseHeader xmlns="http://im.yahooapis.jp/V201911/Account" xmlns:ns2="http://im.yahooapis.jp/V201911">
      <ns2:service>Account</ns2:service>
      <ns2:requestTime>1574393571063</ns2:requestTime>
      <ns2:timeTakenSeconds>0.2671</ns2:timeTakenSeconds>
    </ResponseHeader>
  </SOAP-ENV:Header>
  <SOAP-ENV:Body>
    <ns2:getResponse xmlns="http://im.yahooapis.jp/V201911" xmlns:ns2="http://im.yahooapis.jp/V201911/Account">
      <ns2:rval>
        <totalNumEntries>3</totalNumEntries>
        <ns2:values>
          <operationSucceeded>true</operationSucceeded>
          <ns2:account>
            <ns2:accountId>1111</ns2:accountId>
            <ns2:accountName>SampleAccount</ns2:accountName>
            <ns2:accountType>PREPAY</ns2:accountType>
            <ns2:accountStatus>SERVING</ns2:accountStatus>
            <ns2:deliveryStatus>ACTIVE</ns2:deliveryStatus>
            <ns2:autoTaggingEnabled>FALSE</ns2:autoTaggingEnabled>
          </ns2:account>
        </ns2:values>
        <ns2:values>
          <operationSucceeded>true</operationSucceeded>
          <ns2:account>
            <ns2:accountId>1111</ns2:accountId>
            <ns2:accountName>SampleAccount2</ns2:accountName>
            <ns2:accountType>INVOICE</ns2:accountType>
            <ns2:accountStatus>SERVING</ns2:accountStatus>
            <ns2:deliveryStatus>ACTIVE</ns2:deliveryStatus>
            <ns2:budget>
              <ns2:amount>5000</ns2:amount>
              <ns2:limitChargeType>MONTHLY</ns2:limitChargeType>
              <ns2:startDate>20120529</ns2:startDate>
              <ns2:endDate>20371231</ns2:endDate>
            </ns2:budget>
            <ns2:autoTaggingEnabled>FALSE</ns2:autoTaggingEnabled>
          </ns2:account>
        </ns2:values>
        <ns2:values>
          <operationSucceeded>true</operationSucceeded>
          <ns2:account>
            <ns2:accountId>3333</ns2:accountId>
            <ns2:accountName>SampleAccount3</ns2:accountName>
            <ns2:accountType>PREPAY</ns2:accountType>
            <ns2:accountStatus>SERVING</ns2:accountStatus>
            <ns2:deliveryStatus>ACTIVE</ns2:deliveryStatus>
            <ns2:autoTaggingEnabled>FALSE</ns2:autoTaggingEnabled>
            <ns2:accountAuthorities>VIDEO_VIEW</ns2:accountAuthorities>
            <ns2:accountAuthorities>ITEM_LIST</ns2:accountAuthorities>
            <ns2:accountAuthorities>WEBSITE_TRAFFIC</ns2:accountAuthorities>
            <ns2:accountAuthorities>APP_PROMOTION</ns2:accountAuthorities>
            <ns2:accountAuthorities>CONVERSION</ns2:accountAuthorities>
          </ns2:account>
        </ns2:values>
      </ns2:rval>
    </ns2:getResponse>
  </SOAP-ENV:Body>
</SOAP-ENV:Envelope>
```

## mutate(SET)

### リクエスト

アカウントの情報を操作します。

| パラメータ | 必須 | データ型 |
| ---------- | ---- | -------- |
| operations | Yes | [AccountOperation](../data/Account/AccountOperation.md) |

##### ＜リクエストサンプル＞
```xml
<SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/">
  <SOAP-ENV:Header>
    <RequestHeader xmlns="http://im.yahooapis.jp/V201911/Account" xmlns:ns2="http://im.yahooapis.jp/V201911">
      <ns2:license>1111-1111-1111-1111</ns2:license>
      <ns2:apiAccountId>2222-2222-2222-2222</ns2:apiAccountId>
      <ns2:apiAccountPassword>password</ns2:apiAccountPassword>
    </RequestHeader>
  </SOAP-ENV:Header>
  <SOAP-ENV:Body>
    <mutate xmlns="http://im.yahooapis.jp/V201911/Account">
      <operations>
        <operator>SET</operator>
        <operand>
          <accountId>1111</accountId>
          <accountName>SampleAccount_UpdatedOn</accountName>
          <deliveryStatus>ACTIVE</deliveryStatus>
          <autoTaggingEnabled>TRUE</autoTaggingEnabled>
        </operand>
      </operations>
    </mutate>
  </SOAP-ENV:Body>
</SOAP-ENV:Envelope>
```

### レスポンス

| パラメータ | データ型 |
| -------- | ------- |
| rval | [AccountReturnValue](../data/Account/AccountReturnValue.md) |

##### ＜レスポンスサンプル＞
```xml
<SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/">
  <SOAP-ENV:Header>
    <ResponseHeader xmlns="http://im.yahooapis.jp/V201911/Account" xmlns:ns2="http://im.yahooapis.jp/V201911">
      <ns2:service>Account</ns2:service>
      <ns2:requestTime>1574393571121</ns2:requestTime>
      <ns2:timeTakenSeconds>0.2671</ns2:timeTakenSeconds>
    </ResponseHeader>
  </SOAP-ENV:Header>
  <SOAP-ENV:Body>
    <ns2:mutateResponse xmlns="http://im.yahooapis.jp/V201911" xmlns:ns2="http://im.yahooapis.jp/V201911/Account">
      <ns2:rval>
        <ListReturnValue.Type>AccountReturnValue</ListReturnValue.Type>
        <Operation.Type>SET</Operation.Type>
        <ns2:values>
          <operationSucceeded>true</operationSucceeded>
          <ns2:account>
            <ns2:accountId>1111</ns2:accountId>
            <ns2:accountName>SampleAccount_UpdatedOn</ns2:accountName>
            <ns2:accountType>INVOICE</ns2:accountType>
            <ns2:accountStatus>SERVING</ns2:accountStatus>
            <ns2:deliveryStatus>ACTIVE</ns2:deliveryStatus>
            <ns2:budget>
              <ns2:amount>5000</ns2:amount>
              <ns2:limitChargeType>MONTHLY</ns2:limitChargeType>
              <ns2:startDate>20120529</ns2:startDate>
              <ns2:endDate>20371231</ns2:endDate>
            </ns2:budget>
            <ns2:autoTaggingEnabled>TRUE</ns2:autoTaggingEnabled>
          </ns2:account>
        </ns2:values>
      </ns2:rval>
    </ns2:mutateResponse>
  </SOAP-ENV:Body>
</SOAP-ENV:Envelope>
```

<a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/2.1/jp/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-nd/2.1/jp/">クリエイティブ・コモンズ 表示 - 改変禁止 2.1 日本 ライセンスの下に提供されています。</a>
