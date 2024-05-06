# تونل ED

<p align="left">
  <br><img src="https://github.com/NiREvil/Emotional-Damage/assets/126243832/66c9bdfb-9e74-4a91-a7d3-9a180450c690" width="320px">
</p>

###### با تشکر فراوان از عزیز 3KmFi6HP

[![Repository](https://img.shields.io/badge/View%20on-GitHub-blue.svg)](https://github.com/3Kmfi6HP/EDtunnel)![rainbow](https://github.com/NiREvil/vless/assets/126243832/1aca7f5d-6495-44b7-aced-072bae52f256)

## فهرست مطالب

-   [استقرار در pages.dev](#Deploy-in-pages.dev)
-   [استقرار در worker.dev](#Deploy-in-worker.dev)
-   [تنبلی برای استقرار](#Lazy-to-deploy)
-   [تنظیمات UUID](#UUID-Setting)
    -   [مثال تنظیم UUID](#UUID-Setting-Example)
-   [اشتراک vless لینک](#Subscribe-vless-link)
-   [اشتراک بهترین لینک Cloudflare](#Subscribe-Cloudflare-bestip-link)
-   [پشتیبانی از چند پورت](#Multiple-port-support)
-   [آی پی پروکسی](#ProxyIP)![rainbow](https://github.com/NiREvil/vless/assets/126243832/1aca7f5d-6495-44b7-aced-072bae52f256)

## استقرار در pages.dev

1.  ویدیوی یوتیوب را ببینید:

    [youtube.com/watch](https://www.youtube.com/watch?v=8I-yTNHB0aw)

2.  این استقرار مخزن را در صفحات cloudflare کلون کنید.

## استقرار در worker.dev

1.  کپی 🀄`_worker.js`کد از[اینجا](_worker.js).

2.  همچنین، می‌توانید روی دکمه زیر کلیک کنید تا مستقیماً مستقر شود.

    [![Deploy to Cloudflare Workers](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/NiREvil/Emotional-Damage)

## تنبلی برای استقرار

`aHR0cHM6Ly9vc3MudjJyYXlzZS5jb20vcHJveGllcy9kYXRhLzIwMjMtMDctMzAvRnJFS1lvQS50eHQ=`(پیکربندی اشتراک رایگان clash.meta)

## تنظیمات UUID

1.  هنگام استقرار در صفحات cloudflare، می توانید uuid را در آن تنظیم کنید`wrangler.toml`فایل. نام متغیر است`UUID`.`wrangler.toml`فایل نیز پشتیبانی می شود. (توصیه می شود) در صورت استقرار در صفحات وب، نمی توانید uuid را در آن تنظیم کنید`wrangler.toml`فایل.

2.  هنگام استقرار در worker.dev، می توانید uuid را در آن تنظیم کنید`_worker.js`فایل. نام متغیر است`userID`.`wrangler.toml`فایل نیز پشتیبانی می شود. (توصیه می شود) در صورت استقرار در صفحات وب، نمی توانید uuid را در آن تنظیم کنید`wrangler.toml`فایل. در این حالت می توانید uuid را نیز تنظیم کنید`UUID`متغیر محیطی.

توجه داشته باشید:`UUID`uuid است که می خواهید تنظیم کنید. روش pages.dev و worker.dev همه آنها پشتیبانی می شود، اما به روش استقرار شما بستگی دارد.

### مثال تنظیم UUID

1.  متغیر محیطی تک uuid

    ```.environment
    UUID = "uuid here your want to set"
    ```

2.  چند متغیر محیطی uuid

    ```.environment
    UUID = "uuid1,uuid2,uuid3"
    ```

    توجه: uuid1، uuid2، uuid3 با کاما از هم جدا می شوند`,`.
    وقتی چند uuid را تنظیم می کنید، می توانید استفاده کنید`https://edtunnel.pages.dev/uuid1`برای دریافت پیوند clash config و vless://.

## اشتراک vless لینک

1.  بازدید کنید`https://edtunnel.pages.dev/uuid your set`برای دریافت لینک اشتراک

2.  بازدید کنید`https://edtunnel.pages.dev/sub/uuid your set`برای دریافت محتوای اشتراک با`uuid your set`مسیر.

    توجه داشته باشید:`uuid your set`uuid است که در محیط UUID یا تنظیم کرده اید`wrangler.toml`,`_worker.js`فایل.
    وقتی چند uuid را تنظیم می کنید، می توانید استفاده کنید`https://edtunnel.pages.dev/sub/uuid1`برای دریافت محتوای اشتراک با`uuid1`مسیر. (فقط از اولین uuid در مجموعه uuid چندگانه پشتیبانی می کند)

3.  بازدید کنید`https://edtunnel.pages.dev/sub/uuid your set/?format=clash`برای دریافت محتوای اشتراک با`uuid your set`مسیر و`clash`قالب محتوا با کد base64 باز خواهد گشت.

    توجه داشته باشید:`uuid your set`uuid است که در محیط UUID یا تنظیم کرده اید`wrangler.toml`,`_worker.js`فایل.
    وقتی چند uuid را تنظیم می کنید، می توانید از آن استفاده کنید`https://edtunnel.pages.dev/sub/uuid1/?format=clash`برای دریافت محتوای اشتراک با`uuid1`مسیر و`clash`قالب. (فقط از اولین uuid در مجموعه uuid چندگانه پشتیبانی می کند)

## اشتراک بهترین لینک Cloudflare

1.  بازدید کنید`https://edtunnel.pages.dev/bestip/uuid your set`برای دریافت اطلاعات اشتراک

2.  لینک url اشتراک cpoy`https://edtunnel.pages.dev/bestip/uuid your set`به هر کلاینت (clash/v2rayN/v2rayNG) که می خواهید استفاده کنید.

3.  انجام شده. اگر سوالی دارید لطفا بپیوندید[@edtunnel](https://t.me/edtunnel)یا[@F_NiREvil](https://t.me/F_NiREvil)

## پشتیبانی از چند پورت

   <!-- let portArray_http = [80, 8080, 8880, 2052, 2086, 2095];
	let portArray_https = [443, 8443, 2053, 2096, 2087, 2083]; -->

برای لیستی از پورت های پشتیبانی شده از Cloudflare، لطفاً به آدرس زیر مراجعه کنید[اسناد رسمی](https://developers.cloudflare.com/cloudflare-one/connections/connect-apps/ports).

به طور پیش فرض، پورت 80 و 443 است. اگر می خواهید پورت های بیشتری اضافه کنید، می توانید از پورت های زیر استفاده کنید:

```text
80, 8080, 8880, 2052, 2086, 2095, 443, 8443, 2053, 2096, 2087, 2083
http port: 80, 8080, 8880, 2052, 2086, 2095
https port: 443, 8443, 2053, 2096, 2087, 2083
```

اگر در صفحات cloudflare مستقر می شوید، پورت https پشتیبانی نمی شود. به سادگی چندین پورت را اضافه کنید و از لینک اشتراک استفاده کنید، محتوای اشتراک همه پورت های پشتیبانی شده از Cloudflare را برمی گرداند.

## آی پی پروکسی

1.  هنگام استقرار در صفحات cloudflare، می توانید پروکسی IP را در آن تنظیم کنید`wrangler.toml`فایل. نام متغیر است`PROXYIP`.

2.  هنگام استقرار در worker.dev، می توانید پروکسی IP را در آن تنظیم کنید`_worker.js`فایل. نام متغیر است`proxyIP`.

![rainbow](https://github.com/NiREvil/vless/assets/126243832/1aca7f5d-6495-44b7-aced-072bae52f256)![rainbow](https://github.com/NiREvil/vless/assets/126243832/1aca7f5d-6495-44b7-aced-072bae52f256)نحوه پیدا کردن پروکسی[(منبع)](https://github.com/NiREvil/vless/edit/main/sub/ProxyIP.md)![rainbow](https://github.com/NiREvil/vless/assets/126243832/1aca7f5d-6495-44b7-aced-072bae52f256)![rainbow](https://github.com/NiREvil/vless/assets/126243832/1aca7f5d-6495-44b7-aced-072bae52f256)توجه داشته باشید:`proxyIP`آی پی یا دامنه ای است که می خواهید تنظیم کنید. این بدان معنی است که پروکسی IP برای هدایت ترافیک از طریق یک پروکسی به جای مستقیم به وب سایتی که از Cloudflare (CDN) استفاده می کند استفاده می شود. اگر این متغیر را تنظیم نکنید، اتصال به IP Cloudflare لغو (یا مسدود می شود)...

دلایل: سوکت های خروجی TCP به محدوده IP Cloudflare به طور موقت مسدود شده اند، لطفاً به[اسناد tcp-sockets](https://developers.cloudflare.com/workers/runtime-apis/tcp-sockets/#considerations)

## استفاده

ابتدا دامنه pages.dev خود را باز کنید`https://edtunnel.pages.dev/`در مرورگر خود می توانید صفحه زیر را مشاهده کنید:
مسیر`/uuid your seetting`برای دریافت پیوند clash config و vless://.

![rainbow](https://github.com/NiREvil/vless/assets/126243832/1aca7f5d-6495-44b7-aced-072bae52f256)وام:[آن را استریل کنید](https://github.com/3Kmfi6HP/EDtunnel)&[zizifn](https://github.com/zizifn/edgetunnel)
