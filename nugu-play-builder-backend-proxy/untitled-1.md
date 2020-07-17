---
description: 수면 유도 서비스
---

# StartSleepAction

{% api-method method="post" host="http://stac.gondr.net" path="/nugu/StartSleepAction" %}
{% api-method-summary %}
StartSleepAction
{% endapi-method-summary %}

{% api-method-description %}
NUGU SDK
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{ output: "수면유도를 시작하겠습니다." } or { output: "4 7 8 호흡법을 시작하겠습니다." }
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{output: "연결 실패 했습니다."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

