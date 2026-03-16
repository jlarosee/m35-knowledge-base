# Contacts that crashed DE

- contact#8febc6a111382dd9ac34c30e780a47da
  - no email
- contact#6d9140138131642b575e87de025f58c8
  - no email (not much of anything)
- contact#60daa1d16935bc0001c98a0f
  - nearly empty profile

- contact#5x5-000a9ef0978b821c594450bdc044ec26
  - enrich data but no email

{
 "id": "routerConfig#latest",
 "sortKey": "routerConfig",
 "coldOpenMinimumClicks": 0,
 "coldOpenMinimumOpens": 2,
 "coldPositiveMinimumClicks": 1,
 "coldPositiveMinimumOpens": 2,
 "coldPositiveQueuePinningPeriodDays": 180,
 "coldRiskyInboxThrottlingEnabled": true,
 "gmass5Active": true,
 "gmass5LowRiskProportionThreshold": 0.15,
 "gmass5RiskySMTPProportionThreshold": 0.1,
 "gmass6Active": true,
 "gmass6BatchProportionThreshold": 0.3,
 "gmass6DailySendLimit": 2500,
 "gmass6LowRiskProportionThreshold": 0.2,
 "gmass6QueuePinningPeriodDays": 180,
 "historicEngagementDays": 180,
 "mailjetActive": true,
 "mailjetLowRiskProportionThreshold": 0.3,
 "mailjetRiskySMTPProportionThreshold": 0.3,
 "maxPinAttempts": 3,
 "maxPinnedEmailSendAttempts": 5,
 "pinnedEmailBlackoutDays": 90,
 "riskyInboxProviderMaxSendProportion": 0.4,
 "riskyInboxProviders": [
  "microsoft",
  "mimecast"
 ],
 "riskyInboxProviderSendRatio": {
  "microsoft": {
   "enabled": true,
   "ratio": 0.4
  },
  "mimecast": {
   "enabled": true,
   "ratio": 0.4
  }
 },
 "riskySmtpProviderMaxSendProportion": 0.4,
 "riskySmtpProviders": [
  "microsoft",
  "mimecast"
 ],
 "routeDroppedColdPositiveToCold": true,
 "useRouting": true
}

