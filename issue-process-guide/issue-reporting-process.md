# Issue reporting process

## Metrics

- Severity
  - How does it impact the user experience/features
  - Decided by the tester, according to feature/function list, for example:
    - S1: feature/system is not working, block the workflow
    - S2: feature/system is working with some defects, not blocking the workflow
    - S3: feature/system is working with minor defects, not blocking the workflow
- Frequency
  - How frequently do the defects appear?
  - It's a factor that will impact the decision of priority, or defer a defect.
  - The same symptom with a high reproduction rate (8/10) and low reproduction rate (1/10, or once) will be different priorities.
- Reference
  - [Service Level Agreements](https://www.calibreone.com.au/service-level-agreements/)
  - [Organizing issues with priority to optimize delivery](https://www.atlassian.com/blog/jira-software/organizing-issues-priority-optimize-delivery)

## Bug Report Template

```text
SYMPTOM / 問題の概要
SEVERITY / 深刻度 (choose one)
S1 - features blocked
S2 - bad user experience
S3 - small flaw, need improvement
FREQUENCY / 発生率 (%)
VERSIONS USED / 発生環境
- Pretia SDK Version / Pretia SDKバージョン:
- Device manufacturer, model, and OS / メーカー名, モデル名, OS:
- Output of adb logcat / ログ（adb logcatの出力）:
STEPS TO REPRODUCE THE ISSUE & FREQUENCY / 再現方法
WORKAROUNDS (IF ANY) (HOW TO RECOVER?) / 遭遇した際の回避策（もしあれば）
ADDITIONAL COMMENTS / 備考
```
