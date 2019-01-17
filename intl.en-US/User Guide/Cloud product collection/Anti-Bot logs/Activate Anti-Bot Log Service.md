# Activate Anti-Bot Log Service {#concept_obb_qxt_cgb .concept}

With Anti-Bot Log Service, you can collect multiple log entries in real time from your websites that are protected by the Anti-Bot Service. You can also perform real-time log query and analysis and display results in dashboards.

Based on the website access and attack logs, you can do real-time analysis and research in the Anti-Bot Service management console to assist your security managers in configuring protection policies.

## Procedure {#section_v2q_zxt_cgb .section}

1.  Log on to the [Anti-Bot Service management console](https://partners-intl.console.aliyun.com/#/antibot).
2.  Go to **Report** \> **Log Service**, and select the region of your instance.

    **Note:** You need to click **Authorize** and complete the authorization process to authorize Anti-Bot Service to write log entries to your exclusive logstore, if this is the first time that you use Anti-Bot Log Service.

3.  Click the site Domain drop-down box, select the website domain for which you want to enable the Log Service, and turn on the status switch.

    **Note:** The Domain drop-down list displays all the website domains that are protected by your Anti-Bot Service instance.


Now, you activate the Log Service for the website domain successfully. Log Service automatically creates a dedicated log library and a dedicated logstore for your Alibaba Cloud account. Anti-Bot Service automatically writes all log entries of activated website domains to the exclusive logstore \(antibot-logstore \).

Then, you can retrieve and analyze the access logs for the website domains.

## Limits and instructions {#section_fzx_gzt_cgb .section}

-   Other data cannot be written to the exclusive logstore.

    **Note:** Log entries generated by Anti-Bot Service are stored in the exclusive logstore. You cannot write other data to this logstore by using API, SDK or other methods.

-   Basic configurations, such as the storage period of log entries, cannot be modified.
-   Do not delete or modify the configurations of the project, logstore, index, and dashboards, which are created by Log Service by default.
-   Log Service updates the log query and analysis service on an irregular basis. The index of the exclusive logstore and the default reports are also updated automatically.
-   If you want to use the Anti-Bot log query and analysis service with a RAM user, you must grant the required Log Service permissions to the RAM user.
