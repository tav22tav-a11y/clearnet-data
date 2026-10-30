# ClearNet Privacy Policy / Политика конфиденциальности ClearNet

**Effective date / Дата вступления в силу:** 30 October 2026 / 30 октября 2026 г.  
**Policy version / Версия политики:** 2026-10-30

---

## English

### 1. Purpose and scope
ClearNet is an on-device ad-domain filtering app for selected games. It uses Android's local `VpnService`. ClearNet is not a remote VPN service, does not change your apparent location, and does not route traffic through a ClearNet-operated remote server.

### 2. Data processed locally on the device
To identify games, ClearNet reads the launchable apps visible to Android and package metadata such as package names, labels, categories, and local APK files. APK files may be inspected locally for common game-engine markers.

ClearNet stores selected or disabled game package names, downloaded filter lists, locally observed DNS domain candidates, ad-domain counters, and confirmed learned ad-domain candidates. These items are used only to provide and improve filtering on that device.

### 3. DNS processing and external providers
DNS requests for blocked domains are answered locally with `NXDOMAIN`. DNS requests that are not blocked are sent using DNS-over-HTTPS, first to **Google Public DNS** (`dns.google`) and, if necessary, to **Cloudflare DNS** (`cloudflare-dns.com`). Those providers necessarily receive the DNS query and ordinary network metadata such as the source IP address under their own privacy terms. ClearNet does not control how those independent providers process their server-side logs.

Provider information:
- Google Public DNS privacy information: https://developers.google.com/speed/public-dns/privacy
- Cloudflare public DNS privacy information: https://developers.cloudflare.com/1.1.1.1/privacy/public-dns-resolver/

### 4. Filter-list and game-list updates
ClearNet downloads public filtering and game-package lists from **jsDelivr** and **GitHub**. These services may receive ordinary connection metadata, such as IP address and user agent, when the app checks for updates. ClearNet does not intentionally send your locally selected games or locally learned domain list to these services.

Provider information:
- jsDelivr privacy information: https://www.jsdelivr.com/terms/privacy-policy-jsdelivr-net
- GitHub privacy statement: https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement

### 5. VPN traffic
Only apps placed in ClearNet's allowed VPN list use the local VPN. This normally includes detected or selected games. On Huawei devices, the Huawei ID system component may also be included for compatibility with game services.

Non-DNS TCP and UDP traffic is forwarded directly to its original destination. ClearNet does not decrypt HTTPS content and does not intentionally store application traffic payloads.

### 6. Data ClearNet does not collect
ClearNet does not require a ClearNet account and does not include an analytics or advertising SDK. It does not intentionally collect contacts, photos, microphone recordings, precise location, advertising identifiers, payment-card data, or account passwords. ClearNet does not sell user data.

### 7. Storage, backup, and retention
ClearNet stores the settings and learned filtering data described above in the app's private local storage. Sensitive learned-domain data and game-selection settings are excluded from Android cloud backup and device transfer by the app's backup rules.

Local data remains until it is replaced by normal app operation, app data is cleared, or the app is uninstalled.

### 8. Consent and withdrawal
ClearNet requires acceptance of the current privacy-policy version before it displays detected games or enables VPN filtering. Consent can be withdrawn from the in-app Privacy Policy screen. Withdrawal disables requested protection and returns the app to the consent screen. You may also clear app data or uninstall ClearNet.

### 9. Children
ClearNet is not designed to intentionally collect personal information from children. Where local law requires parental or guardian consent for this processing, ClearNet should only be used with that consent.

### 10. Changes
If this policy changes materially, ClearNet can change the policy version and request a new acceptance before processing resumes.

### 11. Operator and contact
ClearNet is published by **Anton**, the developer name shown on the official app-store listing.

Privacy requests can be submitted through the public ClearNet data repository on GitHub:  
https://github.com/tav22tav-a11y/clearnet-data/issues

---

## Русский

### 1. Назначение и область действия
ClearNet — приложение для локальной фильтрации рекламных доменов в выбранных играх. Оно использует локальный Android `VpnService`. ClearNet не является удалённым VPN-сервисом, не изменяет видимое местоположение пользователя и не направляет трафик через удалённый сервер, управляемый ClearNet.

### 2. Данные, обрабатываемые локально на устройстве
Для определения игр ClearNet читает список запускаемых приложений, который Android делает видимым приложению, и локальные сведения о пакетах: имена пакетов, названия, категории и локальные APK-файлы. APK-файлы могут локально проверяться на наличие известных признаков игровых движков.

ClearNet хранит на устройстве имена выбранных или отключённых игровых пакетов, загруженные списки фильтрации, локально замеченные DNS-домены-кандидаты, счётчики рекламных доменов и подтверждённые обученные рекламные домены. Эти данные используются только для работы и улучшения фильтрации на данном устройстве.

### 3. DNS и внешние провайдеры
DNS-запросы к заблокированным доменам обрабатываются локально ответом `NXDOMAIN`. Разрешённые DNS-запросы передаются по DNS-over-HTTPS сначала в **Google Public DNS** (`dns.google`), а при необходимости — в **Cloudflare DNS** (`cloudflare-dns.com`). Эти независимые провайдеры неизбежно получают сам DNS-запрос и обычные сетевые метаданные, например исходный IP-адрес, в соответствии со своими условиями конфиденциальности. ClearNet не управляет тем, как они обрабатывают серверные журналы.

Информация провайдеров:
- Google Public DNS: https://developers.google.com/speed/public-dns/privacy
- Cloudflare Public DNS: https://developers.cloudflare.com/1.1.1.1/privacy/public-dns-resolver/

### 4. Обновление списков
ClearNet загружает публичные списки фильтрации и игровые списки с **jsDelivr** и **GitHub**. При проверке обновлений эти сервисы могут получать обычные сетевые метаданные, например IP-адрес и User-Agent. ClearNet намеренно не отправляет туда список выбранных пользователем игр или локально обученный список доменов.

Информация провайдеров:
- jsDelivr: https://www.jsdelivr.com/terms/privacy-policy-jsdelivr-net
- GitHub: https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement

### 5. VPN-трафик
Через локальный VPN проходят только приложения, помещённые ClearNet в разрешённый список VPN. Обычно это обнаруженные или выбранные игры. На устройствах Huawei для совместимости с игровыми сервисами в этот список также может включаться системный компонент HUAWEI ID.

TCP- и UDP-трафик, не являющийся DNS, пересылается напрямую исходному назначению. ClearNet не расшифровывает HTTPS-содержимое и намеренно не сохраняет содержимое сетевого трафика приложений.

### 6. Что ClearNet не собирает
ClearNet не требует отдельной учётной записи ClearNet и не содержит SDK аналитики или рекламы. Приложение намеренно не собирает контакты, фотографии, записи микрофона, точное местоположение, рекламные идентификаторы, данные банковских карт или пароли учётных записей. ClearNet не продаёт пользовательские данные.

### 7. Хранение, резервное копирование и срок хранения
Описанные выше настройки и данные обучения хранятся в приватном локальном хранилище приложения. Чувствительные обученные домены и настройки выбора игр исключены правилами ClearNet из облачного резервного копирования Android и переноса на другое устройство.

Локальные данные сохраняются до их обычного обновления приложением, очистки данных приложения или удаления ClearNet.

### 8. Согласие и его отзыв
ClearNet требует согласия с текущей версией политики до отображения обнаруженных игр и включения VPN-фильтрации. Согласие можно отозвать на экране «Политика конфиденциальности». После отзыва запрошенная защита отключается, а приложение возвращается к экрану согласия. Пользователь также может очистить данные приложения или удалить ClearNet.

### 9. Дети
ClearNet не предназначен для намеренного сбора персональной информации детей. Если применимое законодательство требует согласия родителя или законного представителя на такую обработку, ClearNet следует использовать только при наличии такого согласия.

### 10. Изменения
При существенном изменении этой политики ClearNet может изменить номер версии политики и запросить новое согласие до возобновления обработки.

### 11. Оператор и связь
ClearNet публикуется разработчиком **Anton** — это имя разработчика, указанное на официальной странице приложения в магазине.

Запросы по вопросам конфиденциальности можно направить через публичный репозиторий данных ClearNet на GitHub:  
https://github.com/tav22tav-a11y/clearnet-data/issues
