***

**Интеграция** комнаты с каким-то сервисом позволяет или автоматически направлять генерируемые этим сервисом сообщения в эту комнату, и/или направлять опубликованные в этой комнате сообщения в эти сервисы.

В Kato имеется два типа интеграций:

 - [Внутренняя интеграция с журналом аудита](/articles/ru/rooms/integrations#audit-log)
 - [Интеграции с внешними сервисами](/articles/ru/rooms/integrations#list)

## <a href="#audit-log" name="audit-log">![icon_audit](https://s3.amazonaws.com/kato-share/1ff1ab2420539f3d4d5b008f957e047bac4f06c45c9d08ebd288dc34975a965b/clip.png) Внутренняя интеграция с журналом аудита</a>

В комнате, к которой подключена интеграция с **журналом аудита**, автоматически публикуется информация об определённых событиях в данной команде (например, о создании новых комнат или приглашении новых участников). Больше комната с подключённым журналом аудита ничем не отличаются от других комнат, то есть она может быть как защищённой, так и общедоступной, она видна в ростерах всех участников, имеющей к ней доступ, и такие участники могут публиковать в ней сообщения.

В списке ниже перечислены регистрируемые журналом аудита события (сообщения о которых автоматически публикуется в комнатах, интегрированных с журналом аудита): 

 - Изменение экранного имени участника
 - Изменение е-адреса участника
 - Выдача участнику прав админа
 - Отзыв прав админа у участника
 - Приглашение участника в команду
 - Принятие приглашение в команду участником 
 - Удаление участника из команды
 - Создание защищённой комнаты
 - Удаление комнаты из команды
 - Смена имени комнаты
 - Изменение доступа участника к защищённой комнате
 - Изменение типа комнаты с защищённой на общедоступную
 - Изменение типа комнаты с общедоступной на защищённую 
 - Включение интеграции с журналом аудита
 - Выключение интеграции с журналом аудита

Включение интеграции с журналом аудита показано [здесь](/articles/ru/faq/list#how-to-integrate-audit-log).

Только админ может включить интеграцию с журналом аудита к некоторой комнате. Мы рекомендуем создать новую комнату (защищённую или общедоступную). Лучше всего дать этой комнате «говорящее» название, например _Журнал аудита_. Включить интеграцию следует в окне "Manage integrations" этой комнаты:

 ![clip.png](http://i.imgur.com/HDigdhv.png)

## <a href="#list" name="list">Интеграции с внешними сервисами.</a>

***

### <a href="#http_post" name="http_post">![clip.png](https://s3.amazonaws.com/kato-share/99274149d925695cd0677f15d0ef2b05d78cdd8cc6a767ef439edcc91978b83/clip.png) HTTP POST</a>
<br />
Разработчики внешних сервисов могут создавать собственные интеграции с Kato благодаря этой интеграции, позволяющей отправлять отправлять в мессенджер сообщения (POST) в формате JSON.

***

### <a href="#email" name="email">![clip.png](https://s3.amazonaws.com/kato-share/46feccb283936148b37eda00196da0e0f5976d986d029c1c917f334b84d17e1/clip.png) Email</a>
<br />
У каждой комнаты в Kato есть собственный уникальный е-адрес. Поскольку никоторые внешние сервисы поддерживают только оповещения через электронную почту, данную интеграцию можно использовать для перенаправления подобных оповещений в комнаты. 

***

### <a href="#airbrake" name="airbrake">![clip](https://s3.amazonaws.com/kato-share/98755b9c7e3f7b127961ce0f7f43993d14cc18864030142f47e113eb1a0f324/clip.png) Airbrake</a>
<br />
[Airbrake](https://airbrake.io/) — сервис для отслеживания ошибок в сетевых приложениях.

***

### <a href="#appsignal" name="appsignal">![clip.png](https://s3.amazonaws.com/kato-share/1b99fbaee7544174fa85a68dfe4c4c1873ea11c74ec4379e7211783db1a7acb/clip.png) AppSignal</a>
<br />
[AppSignal](https://appsignal.com/) — инструмент для отслеживания ошибок в приложениях на Ruby on Rails. 

***

### <a href="#asana" name="asana">![clip.png](https://s3.amazonaws.com/kato-share/f1fe65fe660b3d67faa458c890970cabf019943810c9521d5e1b518129e92c3b/clip.png) Asana</a>
<br />
[Asana](https://asana.com/) — система для управления проектами и задачами. 

***

### <a href="#balanced" name="balanced">![clip.png](https://s3.amazonaws.com/kato-share/3f568e69f56fbe46d9b7bb0b83c552d8cd59e41ba276edce81f7ea2aece3315f/clip.png) Balanced</a>
<br />
[Balanced](https://www.balancedpayments.com/) — платёжный сервис. 

***

### <a href="#base" name="base">![clip.png](https://s3.amazonaws.com/kato-share/e670dac976be0890f03efe7b5a9995475f5b9ac4e183bc140c17ae625e7ea0b/clip.png) Base CRM</a>
<br />
[Base CRM](https://getbase.com/) — CRM-система, работающая на iOS, Android и Windows Phone. 

***

### <a href="#beanstalk" name="beanstalk">![clip.png](https://s3.amazonaws.com/kato-share/aeff771cb0f2a388a7a1429514f6ca2de8bb9d1f65604006ea20cd21e116464/clip.png) Beanstalk</a>
<br />
[Beanstalk](http://beanstalkapp.com/) — платформа для хостинга репозиториев Git и Subversion и совместной работы над кодом.

***

### <a href="#bitbucket" name="bitbucket">![clip.png](https://s3.amazonaws.com/kato-share/6c585a91af31c18016c69096bbdf1aaded89285bc3af7996c1df067367815ea/clip.png) Bitbucket</a>
<br />
[Bitbucket](https://bitbucket.org) — открытая платформа для хостинга репозиториев Git и Mercurial. 

***

### <a href="#braintree" name="braintree">![clip.png](https://s3.amazonaws.com/kato-share/81fab368d10560c9ba2227a52f294946716f8413d135052017b564a168ead8ed/clip.png) Braintree</a>
<br />
[Braintree](https://www.braintreepayments.com/) — универсальная платежная платформа. 

***

### <a href="#bugsnag" name="bugsnag">![clip.png](https://s3.amazonaws.com/kato-share/c822ed7a8909894ea336b6f4f7ab9788724c0dfca7dad1d72f78091273454ec1/clip.png) Bugsnag</a>
<br />
[Bugsnag](https://bugsnag.com/) — сервис для отслеживания ошибок в сетевых и мобильных приложениях.

***

### <a href="#circleci" name="circleci">![clip.png](https://s3.amazonaws.com/kato-share/b0f1a75903102af3ca698b42d1ae3575dc384d2a8761a60a8da1c4d9f92fa76/clip.png) CircleCI</a>
<br />
[CircleCI](https://circleci.com/) — сервис поддержки непрерывной интеграции для сетевых приложений.

***

### <a href="#cloudforge" name="cloudforge">![clip.png](https://s3.amazonaws.com/kato-share/35c4c415fda49e17a621360b6039b3b172eb6215d2df6ffadf89c4deecb4de38/clip.png) CloudForge</a>
<br />
[CloudForge](http://www.cloudforge.com/) — платформа для хостинга Subversion и Git, а такде для поддержки работы над ошибками.

***

### <a href="#codeship" name="codeship">![clip.png](https://s3.amazonaws.com/kato-share/7a8e15a6fb956d6dc8a03debaac5d31d8f9509d2ea129e39d6dafaeb1fdd73a3/clip.png) Codeship</a>
<br />
[Codeship](https://twitter.com/moritzplassnig) — сервис поддержки непрерывной интеграции. 

***

### <a href="#crashlytics" name="crashlytics">![clip.png](https://s3.amazonaws.com/kato-share/b321aa3e1c69f3c114bbea31bfc72799e12ed1dd49e679fb8efae55c02a95ac/clip.png) Crashlytics</a>
<br />
[Crashlytics](http://try.crashlytics.com/) — сервис для оповещения об отказах мобильных приложений. 

***

### <a href="#customerio" name="customerio">![clip.png](https://s3.amazonaws.com/kato-share/a9e52d2929b42262e89353acf05324f1554be60c616d2fc23d153857131f26a0/clip.png) Customer.io</a>
<br />
[Customer.io](http://customer.io/) — сервис генерации электронных писем на основе поведения пользователей. 

***

### <a href="#desk" name="desk">![clip.png](https://s3.amazonaws.com/kato-share/8797c25e4b980351f26659de37b9bdedafaf68e629d8d179f3d435cd3afed73f/clip.png) Desk</a>
<br />
[Desk](http://www.desk.com/) — приложение для поддержки пользователей.  

***

### <a href="#dokuwiki" name="dokuwiki">![clip.png](https://s3.amazonaws.com/kato-share/e268c4dbde9f08ffb25f8fa32d119eeefc2d60a4149d3ceba0cd62e7ce6ca31c/clip.png) DokuWiki</a>
<br />
[DokuWiki](https://www.dokuwiki.org/dokuwiki) — открытая система для создания вики-страниц, которая работает без базы данных. 

***

### <a href="#doorbell" name="doorbell">![clip.png](https://in.kato.im/9f9d7fce42168fc350d7ef1354e40fe37ceebaf86fd938aeb30e88d6d97d9fbf/clip.png) Doorbell</a>
<br />
[Doorbell](https://doorbell.io) — инструмент для сбора обратной связи от пользователей, встраиваемый в сетевые и  мобильные приложения.

***

### <a href="#freshdesk" name="freshdesk">![clip.png](https://s3.amazonaws.com/kato-share/66391ccf90f055ef9770bf4799d99498a472de3e18175b40af91ea9ec3a84e47/clip.png) Freshdesk</a>
<br />
[Freshdesk](http://freshdesk.com/) — система для поддержки пользователей. 

***

### <a href="#git" name="git">![clip.png](https://s3.amazonaws.com/kato-share/6e17e4193ee9166c93fb72f8c0a5b45eeac71b685c1d2367337384b57d425235/clip.png) Git</a>
<br />
[Git](http://git-scm.com/) — открытая распределённая система версионного контроля.  

***

### <a href="#github" name="github">![clip.png](https://s3.amazonaws.com/kato-share/d2651481d6305741b2d9653a2ef15602d22f9fecb9e588502d5f4306bdd42a5b/clip.png) GitHub</a>
<br />
[GitHub](http://github.com) — платформа для хостинга кода и совместной работы над ним. 

***

### <a href="#gitlab" name="gitlab">![clip.png](https://s3.amazonaws.com/kato-share/1338b03115ee6018568a4d3c1667a3d12628ec4a9367e6c275aa4adce483f668/clip.png) GitLab</a>
<br />
[GitLab](https://about.gitlab.com/) — открытая система для работы с Git. 

***

### <a href="#helpscout" name="helpscout">![clip.png](https://s3.amazonaws.com/kato-share/82956a7c7ce7c693b7753228b447f20b1585305c12c24c3971ef2d0ca3aac0c/clip.png) HelpScout</a>
<br />
[HelpScout](https://www.helpscout.net/) — сервис для специалистов службы поддержки. 

***

### <a href="#heroku" name="heroku">![clip.png](https://s3.amazonaws.com/kato-share/daca62db1a9826b9789929a52863fa85e423a80a3185196be601fbae7b2f28b4/clip.png) Heroku</a>
<br />
[Heroku](https://www.heroku.com/) — платформа для работы с сетевыми приложениями. 

***

### <a href="#hubot" name="hubot">![clip.png](https://in.kato.im/8e0024aca90ceb91828ee90421a4dac4896221f2d449a881701f507b00c70a/clip.png) Hubot</a>
<br />
[Hubot](https://github.com/kato-im/hubot-kato/) — Kato-робот, помогающий автоматизировать многие задачи. К примеру, он может автоматически переводить сообщения с одного языка на другой, или находить в сети прогноз погоды. Страница адаптера Hubot для Kato опубликована на [GitHub](https://github.com/kato-im/hubot-kato). 

***

### <a href="#intercom" name="intercom">![clip.png](https://s3.amazonaws.com/kato-share/c8dd1e4575e38117d804f38216624923e55d38b8b97aecba5d2dd848fcc4bb11/clip.png) Intercom</a>
<br />
[Intercom](https://www.intercom.io/) — сервис, позволяющий сетевым и мобильным проектам общаться со своими пользователями. 

***

### <a href="#ifttt" name="ifttt">![clip.png](https://s3.amazonaws.com/kato-share/75402c164503d0ee1bd4aa7c6a9222b7e7148d3b384a30c81a78d1b35f2acdef/clip.png) IFTTT</a>
<br />
[IFTTT](https://www.ifttt.com/)("if this, then that" — «если это, тогда то») — пользователи IFTTT могут создавать так называемые «рецепты», которые определяют заданный сценарий — что «то» надо сделать, когда наступает «это» событие.

***

### <a href="#jenkins" name="jenkins">![clip.png](https://s3.amazonaws.com/kato-share/b65496a66352826692e830d11d99df48ceef3011b9cfc4eda213052315060b8/clip.png) Jenkins</a>
<br />
[Jenkins](http://jenkins-ci.org/) — открытый сервис для поддержки непрерывной интеграции.

***

### <a href="#jira" name="jira">![clip.png](https://s3.amazonaws.com/kato-share/651d84bd676148c62ef28417485467ca67cf35f7a3e69b9b1e9f62a2a5ed2dd/clip.png) Jira</a>
<br />
[Jira](https://www.atlassian.com/software/jira) — система отслеживания ошибок. 

***

### <a href="#kiln" name="jira">![clip.png](https://s3.amazonaws.com/kato-share/bf3f660925281f8f617b9b3616f71af34fc51539e30cd39571c9a4151b7793f7/clip.png) Kiln</a>
<br />
[Kiln](http://www.fogcreek.com/kiln/) — система управления кодом, основанная на Git и Mercurial.

***

### <a href="#logentries" name="logentries">![clip.png](https://s3.amazonaws.com/kato-share/44545f6c403929ca37a6f9ae31ce5ff01092e648d33529a6beb3f6fd21b6b543/clip.png) LogEntries</a>
<br />
[Logentries](https://logentries.com/) — система для анализа и управления журналами событий.

***

### <a href="#magnumci" name="magnumci">![clip.png](https://s3.amazonaws.com/kato-share/951e35a7dd296f90551ce054414681623d41afbd4ed4ad81bb681d0bf0627b63/clip.png) Magnum CI</a>
<br />
[Magnum CI](https://magnum-ci.com/) — локальная платформа для поддержки непрерывной интеграции и развертывания.

***

### <a href="#mailchimp" name="mailchimp">![clip.png](https://s3.amazonaws.com/kato-share/a8a420d08136e60c1e7b2d6ecda203e3e0e161bcd596d84dc6893eb6747692aa/clip.png) MailChimp</a>
<br />
[MailChimp](http://mailchimp.com/) — платформа для маркетинга средствами электронной почты.

***

### <a href="#mailjet" name="mailjet">![clip.png](https://s3.amazonaws.com/kato-share/eb13ae099a9d743e6208ef9a882427bcacf99345bf4e4db74ec82322871fb4c9/clip.png) Mailjet</a>
<br />
[Mailjet](http://www.mailjet.com/) — система для работы с электронной почтой, поддерживающая маркетинг.

***

### <a href="#mandrill" name="mandrill">![clip.png](https://s3.amazonaws.com/kato-share/c840d8b4cffb93c3a2f0c53986ed47bb83b0af4a0fae68b5705c53088c762bc/clip.png) Mandrill</a>
<br />
[Mandrill](http://mandrill.com/) — транзакционный сервис электронной почты.

***

### <a href="#mention" name="mention">![clip.png](https://s3.amazonaws.com/kato-share/276543ddf4a19cd662fcda0ea9b1a8367eaad92753ba5fe272cbee31e343782f/clip.png) Mention (via Zapier)</a>
<br />
[Mention](https://mention.net/) — система мониторинга средств массовой инфориации.

***

### <a href="#munin" name="munin">![clip.png](https://s3.amazonaws.com/kato-share/f04c2ff549c9bef3f7291cb81a1bb32fa625fe7a3e4c651ddd1f5872731d9fcc/clip.png) Munin</a>
<br />
[Munin](http://munin-monitoring.org/) — система для мониторинга состояния сетей и инфраструктуры.

***

### <a href="#newrelic" name="newrelic">![clip.png](https://s3.amazonaws.com/kato-share/aefd4db09dbb4af8d1a56b8b5e7f764d4193123fb80c2e9322d4d49631a5abcb/clip.png) New Relic</a>
<br />
[New Relic](http://newrelic.com/) — сервис для мониторинга мобильных и сетевых приложений.

***

### <a href="#opsgenie" name="opsgenie">![clip.png](https://s3.amazonaws.com/kato-share/1b07962a3acbadd39b74504023584c4ef7b05943b38a77869259985054c8bc3c/clip.png) OpsGenie</a>
<br />
[OpsGenie](http://www.opsgenie.com/) — система управления оповещениями для мобильных устройств. 

***

### <a href="#pagerduty" name="pagerduty">![clip.png](https://s3.amazonaws.com/kato-share/b0ad622f2fed0b1a1510650d786dc898e22cff5883fac3fd7efa5e11cdbfa73/clip.png) PagerDuty</a>
<br />
[PagerDuty](http://www.pagerduty.com/) — сервис для мониторинга IT-инфраструктуры и контроля инцидентов. 
***

### <a href="#papertrail" name="papertrail">![clip.png](https://s3.amazonaws.com/kato-share/d512a4dbcba12869a69001049901d5cd277cac5d4990b5c37a7db1ea28ec5b6/clip.png) Papertrail</a>
<br />
[Papertrail](https://papertrailapp.com/) — сервис управления журналами событий. 

***

### <a href="#perforce" name="perforce">![clip.png](https://s3.amazonaws.com/kato-share/93469900408a39e8e35a96772d18c779fd7c35817c8ef26fda7bfdb585567fe/clip.png) Perforce</a>
<br />
[Perforce](http://www.perforce.com/) — система для контроля исходного кода. 

***

### <a href="#pingdom" name="pingdom">![clip.png](https://s3.amazonaws.com/kato-share/b099d3855d549ec0da1194117176a486f4832e7c1a452dab5b52055c5f650c7f/clip.png) Pingdom</a>
<br />
[Pingdom](https://www.pingdom.com/) — сервис мониторинга отказов сайтов. 

***

### <a href="#pipedrive" name="pipedrive">![clip.png](https://s3.amazonaws.com/kato-share/13cf48c8284aba25cf90523ba0cb533473ca8eb7125fa7fe6f4817af2767858b/clip.png) Pipedrive</a>
<br />
[Pipedrive](https://www.pipedrive.com/) — сервис для работы с продажами.

***

### <a href="#pivotaltracker" name="pivotaltracker">![clip.png](https://s3.amazonaws.com/kato-share/fc9f76601288a3293f83e974e23f7f9515ee86ffc6751684ab666c6f56b522/clip.png) Pivotal Tracker</a>
<br />
[Pivotal Tracker](http://www.pivotaltracker.com/) — сервис для управления проектами. 

***

### <a href="#postmark" name="postmark">![clip.png](https://s3.amazonaws.com/kato-share/88c69470e991fd6bdd13749e4a5243c224b62c5b77af878cec8b71714f0963cf/clip.png) Postmark</a>
<br />
[Postmark](https://postmarkapp.com/) — сервис email-рассылок для сетевых приложений.

***

### <a href="#raygun" name="raygun">![clip.png](https://s3.amazonaws.com/kato-share/cb2d274682c281dd9228a9cc9d9daded6c3d05fd1a0f26e226dd1613c01d3ba/clip.png) Raygun</a>
<br />
[Raygun](http://raygun.io/) — сервис генерации отчетов об ошибках и отказах в приложениях.

***

### <a href="#redmine" name="redmine">![clip.png](https://s3.amazonaws.com/kato-share/d8cfd902545845045ecd3d9fcd03ea48e4e68c5d40bec238cd8c57480f7c1c8/clip.png) Redmine</a>
<br />
[Redmine](http://www.redmine.org/) — сервис для управления проектами и контроля ошибок.

***

### <a href="#rss" name="rss">![clip.png](https://s3.amazonaws.com/kato-share/ca797c3481ff595633134a56c3720fabba6fc712a38dcf384768ee431402de5f/clip.png) RSS (через Zapier)</a>
<br />
RSS — способ получения информации из различных источников в одном месте.

***

### <a href="#runscope" name="runscope">![clip.png](https://s3.amazonaws.com/kato-share/33be53d65ed8d759e64592cb7d96debd700afe535cce7db06b4b1ca78e4bf766/clip.png) Runscope</a>
<br />
[Runscope](https://www.runscope.com/) – сервис для тестирования API и мониторинга для разработчиков приложений. 

***

### <a href="#semaphore" name="semaphore">![clip.png](https://s3.amazonaws.com/kato-share/49cf1b13a74129e47b357dca90b74f7bb8b110683a6a677ebba95befa525f68/clip.png) Semaphore</a>
<br />
[Sempahore](https://semaphoreapp.com/) – сервис для непрерывной интеграции приложений на Ruby on Rails. 

***

### <a href="#sendgrid" name="sendgrid">![clip.png](https://s3.amazonaws.com/kato-share/3bc2fc729cb0e6f33f59f812db6961a95372aa41795f9bc06d4341ca1d3af3b6/clip.png) SendGrid</a>
<br />
[SendGrid](http://sendgrid.com/) — транзакционный сервис для email-рассылок. 

***

### <a href="#sentry" name="sentry">![clip.png](https://s3.amazonaws.com/kato-share/19485943b69dd49cc389265648d391355378745dfcc65c0ec84be362f7e5971f/clip.png) Sentry</a>
<br />
[Sentry](https://getsentry.com/) — сервис для оповещения об ошибках в мобильных и сетевых приложениях. 

***

### <a href="#shopify" name="shopify">![clip.png](https://s3.amazonaws.com/kato-share/b6e5d1fef9901096b28ea3fb4f637b4ebb4ccf7e21ee403c11678da8327dbe24/clip.png) Shopify</a>
<br />
[Shopify](http://www.shopify.com/) — онлайн-конструктор интернет-магазинов.

***

### <a href="#sprintly" name="sprintly">![clip.png](https://s3.amazonaws.com/kato-share/ac665975bd760dddb3c7321c843a554e621af94286b88c302f120c4bf96289d8/clip.png) Sprintly</a>
<br />
[Sprintly](https://sprint.ly/) — сервис для управления проектами. 

***

### <a href="#stash" name="stash">![clip.png](https://s3.amazonaws.com/kato-share/370138b126961dca482cf7d5976e872af6cd9c0788e53b1ea695775297a031fb/clip.png) Stash</a>
<br />
[Stash](https://www.atlassian.com/software/stash) — инструмент для управления репозиториями Git.

***

### <a href="#stripe" name="stripe">![clip.png](https://s3.amazonaws.com/kato-share/923ea0d6dca569bd864b093fecf0767d7c61ee7c49d1d3b211df7a89b314c99c/clip.png) Stripe</a>
<br />
[Stripe](https://stripe.com) — сервис для организации приема платежей в мобильных и сетевых проектах. 

***

### <a href="#teamcity" name="teamcity">![clip.png](https://s3.amazonaws.com/kato-share/e1ae5659ed45a59d49116e1aa899261665583d22fd5a486e115bb79a171f1705/clip.png) TeamCity</a>
<br />
[TeamCity](http://www.jetbrains.com/teamcity/) — билд-сервер для обеспечения непрерывной интеграции. 

***

### <a href="#tender" name="tender">![clip.png](https://s3.amazonaws.com/kato-share/8793ff3c372ad125b2b7282787b8ddfaa68cc23014e322e7d73ae4a366300a/clip.png) Tender Support</a>
<br />
[Tender Support](http://tenderapp.com/) — база знаний и программное обеспечение для создания форумов, а также инструмент для организации поддержки пользователей.

***

### <a href="#travis" name="travis">![clip.png](https://s3.amazonaws.com/kato-share/dc46e4b8e9e3b6d2d16d9d27d683cc20d70711c6a6761d5c8aad4c39cd4048a/clip.png) Travis</a>
<br />
[Travis](https://travis-ci.org/) — сервис для поддержки непрерывной интеграции и развертывания. 

***

### <a href="#trello" name="trello">![clip.png](https://s3.amazonaws.com/kato-share/da009d49aa4fae71adb77512c2d386c987629a7bb074d87b2db351972706e10d/clip.png) Trello</a>
<br />
[Trello](https://trello.com/) — сервис для управления проектами и задачами.

***

### <a href="#unbounce" name="unbounce">![clip.png](https://s3.amazonaws.com/kato-share/4b5cd6b14f42ee9f6b05c8525fed03dd5152a0591a08185c9090741d403d2b9/clip.png) Unbounce</a>
<br />
[Unbounce](http://unbounce.com/) — сервис для создания, публикации, альфа-тестирования и бета-тестирования домашних страниц.

***

### <a href="#userecho" name="userecho">![clip.png](https://in.kato.im/dea28f418e245c7415b77c6322f9e8c25567ddbcf6c73568ca36e4bddd443fa5/clip.png) UserEcho</a>
<br />
[UserEcho](https://www.userecho.com/) — сервис для организации поддержки клиентов с встроенным модулем helpdesk, онлайн-чатом, базой знаний и форумом.

***

### <a href="#uservoice" name="uservoice">![clip.png](https://s3.amazonaws.com/kato-share/20a73a22f67040d2798ad6ed98009bc5b9e32d0a8e6470f9e3b87f89786b9eeb/clip.png) UserVoice</a>
<br />
[UserVoice](https://www.uservoice.com/) — инструмент для оказания поддержки пользователей с встроенным helpdesk модулем и базой знаний. 

***

### <a href="#vend" name="vend">![clip.png](https://s3.amazonaws.com/kato-share/7e29c72c33d4ab299281b42b58547630ecaddf52c12dfb4def0ae08e8ea68800/clip.png) Vend</a>
<br />
[Vend](http://www.vendhq.com/) — программное обеспечение и физическое устройство для приема платежей с карточек в торговой сети. 

***

### <a href="#vso" name="vso">![clip.png](https://s3.amazonaws.com/kato-share/817082233ab941dcb3300ca5458f24d436256216da6aafcc374212007ae8c52b/clip.png) Visual Studio Online</a>
<br />
[Visual Studio Online](http://www.visualstudio.com/en-us/products/visual-studio-online-overview-vs) — облачная версия Microsoft Visual Studio.

***

### <a href="#wordpress" name="wordpress">![clip.png](https://s3.amazonaws.com/kato-share/b4b481669764db664b46a5d419bcbfb7f939ef9a44c5524ff722b990250e4a7e/clip.png) WordPress</a>
<br />
[WordPress](http://wordpress.com/) — блогосервис и CMS-система.

***

### <a href="#workingon" name="workingon">![clip.png](https://s3.amazonaws.com/kato-share/ec007f2ba8e37c3f34d0ad93e1e72761b84018b3cf3ce7a25d1b2f60fe03f10a/clip.png) WorkingOn</a>
<br />
[WorkingOn](https://www.workingon.co/) — сервис для отслеживания прогресса в разработке проекта.

***

### <a href="#zapier" name="zapier">![clip.png](https://s3.amazonaws.com/kato-share/16a41c8d3e414e6da3f18ad06ac1b8d68e2eb236d7e30e58bfc6291d03190e/clip.png) Zapier</a>
<br />
[Zapier](http://zapier.com) позволяет интегрировать сотни сервисов. 

***

### <a href="#zendesk" name="zendesk">![clip.png](https://s3.amazonaws.com/kato-share/daea0b10e78fad32a3382fbfa0c8670a914afe09bfde7bd06da0579d1f1f853d/clip.png) Zendesk</a>
<br />
[Zendesk](http://www.zendesk.com/) — система для организации подержки пользователей и создания тикетов. 
